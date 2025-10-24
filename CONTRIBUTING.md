# Contributing to Anomalous Field Recorder

Thank you for your interest in improving Anomalous Field Recorder! This guide explains how to set up your development environment, submit changes, and collaborate with the community.

## Table of Contents

1. [Code of Conduct](#code-of-conduct)
2. [Project Structure](#project-structure)
3. [Development Environment](#development-environment)
4. [Branching Model](#branching-model)
5. [Commit Guidelines](#commit-guidelines)
6. [Testing](#testing)
7. [Documentation](#documentation)
8. [Pull Request Process](#pull-request-process)
9. [Release Process](#release-process)

## Code of Conduct

Participation in this project is governed by the [Code of Conduct](CODE_OF_CONDUCT.md). By contributing, you agree to uphold its principles.

## Project Structure

```
src/                # Core library code
scripts/            # Operational scripts for acquisition and processing
notebooks/          # Jupyter notebooks for analysis
tests/              # Automated test suite
tools/              # Calibration, deployment, and developer tooling
```

Refer to the [README](README.md) for more context on each directory.

## Development Environment

1. Install Python 3.11 or newer.
2. Install Poetry for dependency management.
3. Clone the repository and install dependencies:

   ```bash
   git clone https://github.com/<org>/Anomalous-Field-Recorder.git
   cd Anomalous-Field-Recorder
   poetry install
   ```

4. Activate the virtual environment: `poetry shell` (optional).
5. Install pre-commit hooks:

   ```bash
   poetry run pre-commit install
   ```

### Optional Services

- **Database**: If you require metadata persistence, run `docker compose up db` to start the PostgreSQL instance defined in `docker-compose.yml`.
- **MinIO/S3**: Use `docker compose up object-storage` to emulate remote storage for large datasets.

## Branching Model

- Use `main` for production-ready code.
- Create feature branches from `main` using the pattern `feature/<short-description>`.
- Use `bugfix/<short-description>` for patches.
- Hotfixes should target the latest release tag and be merged back into `main` and the release branch.

## Commit Guidelines

- Write descriptive commit messages in the imperative mood (e.g., "Add spectral denoising filter").
- Keep commits focused and self-contained.
- Reference relevant issues using `Fixes #123` or `Refs #456` in the commit body.
- Avoid committing generated artifacts, large binaries, or secrets.

## Testing

Before submitting a pull request:

```bash
poetry run ruff check .
poetry run mypy src
poetry run pytest
```

Include additional integration or hardware-in-the-loop tests when relevant. Provide links to experiment logs in `docs/experiments/` if your change alters acquisition procedures.

## Documentation

- Update the README, docs, and notebooks when APIs or workflows change.
- Document public functions and classes with type hints and docstrings.
- Keep changelog entries in `docs/changelog.md` organized under the appropriate release heading.

## Pull Request Process

1. Ensure your branch is up to date with `main`.
2. Submit a PR with:
   - Summary of changes
   - Testing performed (commands and results)
   - Any outstanding issues or follow-up tasks
3. Request review from at least one maintainer.
4. Address review feedback promptly and politely.
5. Squash or rebase commits if requested.

## Release Process

- Update version numbers in `pyproject.toml` and related artifacts.
- Draft release notes in `docs/releases/<version>.md` summarizing key changes.
- Ensure CI passes on the release branch.
- Tag the release (`git tag vX.Y.Z`) and push the tag to origin.
- Publish the release on GitHub with links to documentation and datasets.

We appreciate your contributions and look forward to collaborating!

