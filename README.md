# dctl

`dctl` is the Command Line Interface (CLI) for DeployPlex.

[![pypi version](https://img.shields.io/pypi/v/dctl.svg)](https://pypi.org/pypi/dctl/)
[![Downloads](https://static.pepy.tech/badge/dctl/week)](https://pypi.org/pypi/dctl/)
[![License: MIT](https://img.shields.io/badge/license-Apache--2.0-yellow)](https://www.apache.org/licenses/LICENSE-2.0)
[![Twitter](https://img.shields.io/twitter/url/https/x.com/dctl.svg?style=social&label=Follow%20%40deployplex)](https://x.com/deployplex)
[![](https://dcbadge.vercel.app/api/server/BP5aUkhcAh?compact=true&style=flat)](https://discord.com/invite/BP5aUkhcAh)

## Getting Started

### Requirements
- [Python 3.11.2](https://www.python.org/downloads/)

You can install and configure dctl using this command:
```bash
pip install -U dctl
```

Login into deployplex to start using the CLI:
```bash
dctl login
```

Alternatively you can use a deployplex token generated from the dashboard and set it as an environment variable.
```bash
export DEPLOYPLEX_TOKEN="you_deployplex_token"
```

## Usage

On the terminal
```bash
dctl --help
```

On Github Actions
```yaml
steps:
  - name: Checkout Repository
    uses: actions/checkout@v3

  - name: Setup dctl CLI
    uses: deployplex/dctl@0.0.13
    with:
      token: ${{ secrets.DEPLOYPLEX_TOKEN }}
```

## Learn more

The best place to get started is following our getting started guide on the [DeployPlex CLI Documentation](https://docs.deployplex.com/cli).

## LICENSE

`dctl` is published under the [Apache-2.0 license](LICENSE)
