# GitHub Actions Standards

Reusable GitHub Actions workflows for repositories owned by `malabie`.

## Included workflows

- `reusable-security.yml`
  - Gitleaks secret scanning on pushes and pull requests
  - Dependency review on pull requests
  - GitHub Actions workflow linting when workflow files are present
- `reusable-codeql-js.yml`
  - CodeQL scanning for JavaScript and TypeScript repositories

## Usage

Each repository keeps a tiny wrapper workflow in `.github/workflows/` and calls these reusable workflows from this repository.
