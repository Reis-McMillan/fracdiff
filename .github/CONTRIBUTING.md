# Contributing

Any contributions are more than welcome.

* **Issues**: Bug reports, feature requests, and questions.
* **Pull Requests**: Bug-fixes, feature implementations, and documentation updates.

## Development Environment

This project supports **Python 3.8 through 3.13**. To ensure compatibility across all versions, we use [tox](https://tox.wiki/) for automation and [setuptools](https://setuptools.pypa.io/) as the build backend.

### 1. Installation

First, clone the repository and install the package in editable mode with development dependencies:

```sh
git clone [https://github.com/Reis-McMillan/fracdiff-modern.git](https://github.com/Reis-McMillan/fracdiff-modern.git)
cd fracdiff
pip install -e ".[dev,sklearn,torch]"
```

### 2. Testing and Linting

Instead of `Makefile`, we use `tox` to run tests and linters in isolated environments. This ensures the code works across different Python versions.

- Run all tests and linters (requires Python 3.8 and 3.13 to be installed locally):
```bash
pip install tox
tox
```

- Run tests for a specific Python version:
```bash
tox -e py313
```

- Run the linter (Flake 8):
```bash
tox -e lint
```

### 3. Pull Request Guidelines
Before submitting a pull request, pleasue ensure:
1. Your code follows the **Flake8** style guidelines (check this by running `tox -e lint`).
2. All tests have pass on the supported Python versions.
3. You have added or updated tests if you are introducing new features or fixing bugs.
4. If you are preparing a new release, please follow the **Branching Strategy** below.

## Branching Strategy

We use an automated worflow for versioning:
- **Feature/Fix branches**: Branch off `main` and submit PR back to `main`.
- **Release branches**: To trigger an automated version bump, create a branch named `release/X.Y.Z` (e.g., `release/1.1.0`). Our GitHub Actions will automatically update the version in `pyproject.toml` and open a PR for you.