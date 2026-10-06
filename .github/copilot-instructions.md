# Copilot Instructions for Trabalho-titanic

## Project overview
This repository is a very small Python project built around the Seaborn Titanic sample dataset. The current implementation is intentionally minimal: the logic lives in `a.py`, which imports `seaborn` and loads the `titanic` dataset. There is no application package, no service layer, and no multi-module architecture yet.

## Commands
There is no formal build, test, or lint toolchain configured in this repository at the moment.

- Run the script directly:
  - `python a.py`
- There is no `pytest`, `unittest`, `ruff`, `flake8`, `black`, or CI workflow in the repo right now, so there are no repo-wide test or lint commands to document.

## Architecture
- The repository is effectively a single-file exploration script.
- `a.py` is the central entry point and should be treated as the primary place for dataset loading and any analysis logic.
- The project does not currently define classes, modules, or separate responsibilities such as data access, processing, or presentation.
- If the project grows, keep the structure simple and add complexity only when there is a clear need to separate concerns.

## Key conventions
- Keep the repository lightweight; avoid adding framework scaffolding or package structure unless the project clearly needs it.
- Prefer direct Python code over abstraction layers; this project is small and script-oriented.
- When working with data, keep dependencies limited to the existing Seaborn/Python data stack rather than introducing broad app infrastructure.
- Use the README as the canonical source for the repo’s purpose; avoid expanding the project into a larger app without updating documentation.
- Because there is no automated test suite, validation is usually done by running the script or using a focused local check that matches the task.

## Working assumptions
- Changes should remain easy to understand in one file unless there is a real need to split functionality.
- New files should be justified by clear project needs; the current repo does not have a package system to preserve.
- Keep examples and scripts reproducible with the local Python environment rather than depending on a custom build pipeline.
