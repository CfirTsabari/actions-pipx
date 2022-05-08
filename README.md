# actions-pipx
GitHub Actions for using pipx

[![license](https://img.shields.io/github/license/CfirTsabari/actions-pipx.svg)](https://github.com/CfirTsabari/actions-pipx/blob/master/LICENSE)
[![release](https://img.shields.io/github/release/CfirTsabari/actions-pipx.svg)](https://github.com/CfirTsabari/actions-pipx/releases/latest)

- [pypa/pipx: Install and Run Python Applications in Isolated Environments.](https://github.com/pypa/pipx)

> Inspired by [abatilo's](https://www.aaronbatilo.dev/) [poetry action](https://github.com/abatilo/actions-poetry).

## Getting started

### Create your workflow
```yaml
name: CI
on: pull_request

jobs:
  ci:
    runs-on: windows-latest
    steps:
      - uses: actions/checkout@v2
      - uses: actions/setup-python@v2
        with:
          python-version: 3.9
      - name: Run image
        uses: CfirTsabari/actions-pipx@v1
      - name: Run something using pipx
        run: pipx run pycowsay
```

## License
[MIT License - CfirTsabari/actions-pipx](https://github.com/CfirTsabari/actions-pipx/blob/master/LICENSE)


