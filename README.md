# hadolint-coatl

[![PyPI - Version](https://img.shields.io/pypi/v/hadolint-coatl)](https://pypi.org/project/hadolint-coatl)
[![Downloads](https://static.pepy.tech/badge/hadolint-coatl)](https://pepy.tech/project/hadolint-coatl)

A python wrapper to provide a pip-installable [hadolint] binary. Inspired by
[shellcheck-py].

Internally this package provides a convenient way to download the pre-built
hadolint binary for your particular platform.

### installation

```bash
pip install hadolint-coatl
```

### usage

After installation, the `hadolint` binary should be available in your
environment (or `hadolint.exe` on windows).

### As a pre-commit hook

See [pre-commit] for instructions

Sample `.pre-commit-config.yaml`:

```yaml
  - repo: https://github.com/coatl-dev/hadolint-coatl
    rev: 2.12.1b0
    hooks:
      - id: hadolint
```

[hadolint]: https://github.com/hadolint/hadolint
[pre-commit]: https://pre-commit.com
[shellcheck-py]: https://github.com/shellcheck-py/shellcheck-py
