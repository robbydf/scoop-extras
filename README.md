# scoop-extras

[![Tests](https://github.com/robbydf/scoop-extras/actions/workflows/ci.yml/badge.svg)](https://github.com/robbydf/scoop-extras/actions/workflows/ci.yml) [![Excavator](https://github.com/robbydf/scoop-extras/actions/workflows/excavator.yml/badge.svg)](https://github.com/robbydf/scoop-extras/actions/workflows/excavator.yml)

Robby's [Scoop](https://scoop.sh/) bucket for apps that aren't in the main Scoop buckets.

## Installation

Add this bucket to Scoop, then install an app from it:

```powershell
scoop bucket add scoop-extras https://github.com/robbydf/scoop-extras
scoop install scoop-extras/slackcli
```

## Apps

| App | Description | Version |
| --- | --- | --- |
| [slackcli](bucket/slackcli.json) | Command-line tool for interacting with Slack workspaces and channels | [![Version](https://img.shields.io/github/v/release/shaharia-lab/slackcli)](https://github.com/shaharia-lab/slackcli/releases) |
| [gcx](bucket/gcx.json) | CLI for managing Grafana and Grafana Cloud resources | [![Version](https://img.shields.io/github/v/release/grafana/gcx)](https://github.com/grafana/gcx/releases) |

## Updating

```powershell
scoop update
scoop update slackcli
```

## Contributing

Manifests in this bucket are validated automatically on every pull request (lint, hashes, checkver, and autoupdate checks). Before opening a PR:

1. Add or edit a manifest under `bucket/`.
2. Format it with `.\bin\formatjson.ps1 -App <name>`.
3. Verify it installs cleanly: `scoop install bucket/<name>.json`.
