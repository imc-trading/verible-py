[![Build Status](https://dev.azure.com/shellcheck-py/shellcheck-py/_apis/build/status/shellcheck-py.shellcheck-py?branchName=main)](https://dev.azure.com/shellcheck-py/shellcheck-py/_build/latest?definitionId=1&branchName=main)
[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/shellcheck-py/shellcheck-py/main.svg)](https://results.pre-commit.ci/latest/github/shellcheck-py/shellcheck-py/main)

# shellcheck-py

A python wrapper to provide a pip-installable [shellcheck] binary.

Internally this package provides a convenient way to download the pre-built
shellcheck binary for your particular platform.

### installation

```bash
pip install shellcheck-py
```

### usage

After installation, the `shellcheck` binary should be available in your
environment (or `shellcheck.exe` on windows).

### As a pre-commit hook

See [pre-commit] for instructions

Sample `.pre-commit-config.yaml`:

```yaml
-   repo: https://github.com/shellcheck-py/shellcheck-py
    rev: v0.9.0.1
    hooks:
    -   id: shellcheck
```

[shellcheck]: https://shellcheck.net
[pre-commit]: https://pre-commit.com
