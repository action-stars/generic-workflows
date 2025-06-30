# Action Stars Generic Workflows for GitHub Actions

![GitHub Release (latest SemVer)](https://img.shields.io/github/v/release/action-stars/generic-workflows?sort=semver)
![Validate](https://github.com/action-stars/generic-workflows/actions/workflows/_validate.yaml/badge.svg?branch=main)

## Dependabot Changelog Workflow

This GitHub Actions workflow generates a changelog for Dependabot.

<!-- MERGE:START:dependabot-changelog - Do not remove or modify this section -->
### Inputs

<!-- AUTO-DOC-INPUT:START - Do not remove or modify this section -->
No inputs.
<!-- AUTO-DOC-INPUT:END -->
### Outputs

<!-- AUTO-DOC-OUTPUT:START - Do not remove or modify this section -->
No outputs.
<!-- AUTO-DOC-OUTPUT:END -->
<!-- MERGE:END:dependabot-changelog - Do not remove or modify this section -->

## Publish Release Workflow

This GitHub Actions workflow publishes a release.

<!-- MERGE:START:release - Do not remove or modify this section -->
### Inputs

<!-- AUTO-DOC-INPUT:START - Do not remove or modify this section -->

|     INPUT      |  TYPE   | REQUIRED |          DEFAULT           |                                        DESCRIPTION                                        |
|----------------|---------|----------|----------------------------|-------------------------------------------------------------------------------------------|
|   artifacts    | string  |  false   |                            | Comma separated list of artifact path to be uploaded to the release; this supports globs. |
| changelog_path | string  |  false   |     `"./CHANGELOG.md"`     |      Path to the CHANGELOG file; this needs to follow the Keep a Changelog pattern.       |
|  make_latest   | boolean |  false   |           `true`           |                      Whether to make the release the latest release.                      |
|    version     | string  |  false   | `"${{ github.ref_name }}"` |                                The version to be released.                                |

<!-- AUTO-DOC-INPUT:END -->
### Outputs

<!-- AUTO-DOC-OUTPUT:START - Do not remove or modify this section -->
No outputs.
<!-- AUTO-DOC-OUTPUT:END -->
<!-- MERGE:END:release - Do not remove or modify this section -->

## OSSF Scorecard Workflow

This GitHub Actions workflow runs the OSSF Scorecard.

<!-- MERGE:START:scorecard - Do not remove or modify this section -->
### Inputs

<!-- AUTO-DOC-INPUT:START - Do not remove or modify this section -->

|     INPUT      |  TYPE  | REQUIRED | DEFAULT |                   DESCRIPTION                    |
|----------------|--------|----------|---------|--------------------------------------------------|
| retention_days | number |  false   |   `7`   | Number of days to retain the scorecard artifact. |

<!-- AUTO-DOC-INPUT:END -->
### Outputs

<!-- AUTO-DOC-OUTPUT:START - Do not remove or modify this section -->
No outputs.
<!-- AUTO-DOC-OUTPUT:END -->
<!-- MERGE:END:scorecard - Do not remove or modify this section -->

## Validate GitHub Action Workflow

This workflow validates the GitHub Action in the repository.

<!-- MERGE:START:validate-gh-action - Do not remove or modify this section -->
### Inputs

<!-- AUTO-DOC-INPUT:START - Do not remove or modify this section -->

|    INPUT     |  TYPE   | REQUIRED | DEFAULT |          DESCRIPTION           |
|--------------|---------|----------|---------|--------------------------------|
|   auto_doc   | boolean |  false   | `false` |   If auto-doc should be run.   |
| markdownlint | boolean |  false   | `false` | If markdownlint should be run. |
|  shellcheck  | boolean |  false   | `false` |  If shellcheck should be run.  |
|   yamlfmt    | boolean |  false   | `false` |   If yamlfmt should be run.    |

<!-- AUTO-DOC-INPUT:END -->
### Outputs

<!-- AUTO-DOC-OUTPUT:START - Do not remove or modify this section -->
No outputs.
<!-- AUTO-DOC-OUTPUT:END -->
<!-- MERGE:END:validate-gh-action - Do not remove or modify this section -->

## Validate GitHub Workflows Workflow

This workflow validates the GitHub Workflows in the repository.

<!-- MERGE:START:validate-gh-workflows - Do not remove or modify this section -->
### Inputs

<!-- AUTO-DOC-INPUT:START - Do not remove or modify this section -->

|      INPUT      |  TYPE   | REQUIRED | DEFAULT |          DESCRIPTION           |
|-----------------|---------|----------|---------|--------------------------------|
|    auto_doc     | boolean |  false   | `false` |   If auto-doc should be run.   |
| auto_doc_script | string  |  false   |         |  The script to run auto-doc.   |
|  markdownlint   | boolean |  false   | `false` | If markdownlint should be run. |
|   shellcheck    | boolean |  false   | `false` |  If shellcheck should be run.  |
|     yamlfmt     | boolean |  false   | `false` |   If yamlfmt should be run.    |

<!-- AUTO-DOC-INPUT:END -->
### Outputs

<!-- AUTO-DOC-OUTPUT:START - Do not remove or modify this section -->
No outputs.
<!-- AUTO-DOC-OUTPUT:END -->
<!-- MERGE:END:validate-gh-workflows - Do not remove or modify this section -->
