# verible-py

A python wrapper to provide a pip-installable [verible] binary.

Internally this package provides a convenient way to download the pre-built
verible binary for your particular platform.

### installation

```bash
pip install verible-py
```

### usage

After installation, the `verible` binary should be available in your
environment (or `verible.exe` on windows).

### As a pre-commit hook

See [pre-commit] for instructions

Sample `.pre-commit-config.yaml`:

```yaml
- repo: https://github.com/imc-trading/verible-py.git
    rev: v0.0-3824
    hooks:
      - id: verible-verilog-lint
      - id: verible-verilog-format
```

[verible]: https://chipsalliance.github.io/verible/
[pre-commit]: https://pre-commit.com
