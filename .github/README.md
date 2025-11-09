# Matrix Build Workflow

This repository demonstrates a GitHub Actions workflow with matrix build strategy and artifact management.

## Workflow Features

- **Matrix Strategy**: Builds across 3 different OS platforms (Ubuntu, macOS, Windows) and 3 Node.js versions
- **Parallel Execution**: All matrix combinations run simultaneously
- **Artifact Management**: Each job generates and uploads unique build artifacts
- **Artifact Naming**: Artifacts follow the pattern `build-a20bf30-<platform>-node<version>`

## Workflow Details

The workflow (`matrix-build.yml`) includes:
- Matrix build with 9 total combinations (3 OS × 3 Node versions)
- Unique artifact generation for each combination
- Artifact upload using `actions/upload-artifact@v4`
- Step identifier: `matrix-a20bf30`

## Artifact Prefix

All uploaded artifacts use the prefix: `build-a20bf30-`

## Contact

Email: your-email@example.com

## Validation Requirements

- ✅ At least 3 successful matrix jobs
- ✅ At least 3 artifacts uploaded with prefix `build-a20bf30`
- ✅ All artifacts contain actual content (non-empty)
- ✅ Step identifier `matrix-a20bf30` included
- ✅ README.md file with email address
