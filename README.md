# GitHub Actions Standards

Reusable GitHub Actions workflows for repositories owned by `malabie`.

## Included workflows

- `reusable-security.yml`
  - Gitleaks secret scanning on pushes and pull requests
  - Dependency review on pull requests
  - GitHub Actions workflow linting when workflow files are present
- `reusable-codeql-js.yml`
  - CodeQL scanning for JavaScript and TypeScript repositories that support GitHub code scanning

## Usage

Each repository keeps a tiny wrapper workflow in `.github/workflows/` and calls these reusable workflows from this repository.

## Important note for private repositories

GitHub code scanning is not available for user-owned private repositories on GitHub Free or GitHub Pro. Because of that, the shared CodeQL wrapper should only be added to repositories where code scanning is actually available.
