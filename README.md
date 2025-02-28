# Action Stars Generic Workflows for GitHub Actions

## Publish Release Workflow

This GitHub Actions workflow publishes a release.

<!-- MERGE:START:release - Do not remove or modify this section -->
### Inputs

<!-- AUTO-DOC-INPUT:START - Do not remove or modify this section -->

|     INPUT      |  TYPE   | REQUIRED |          DEFAULT           |                                        DESCRIPTION                                        |
|----------------|---------|----------|----------------------------|-------------------------------------------------------------------------------------------|
|   artifacts    | string  |  false   |                            | Comma seperated list of artifact path to be uploaded to the release; this supports globs. |
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
