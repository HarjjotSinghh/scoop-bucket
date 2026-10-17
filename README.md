# scoop-bucket

[![Tests](https://github.com/HarjjotSinghh/scoop-bucket/actions/workflows/ci.yml/badge.svg)](https://github.com/HarjjotSinghh/scoop-bucket/actions/workflows/ci.yml) [![Excavator](https://github.com/HarjjotSinghh/scoop-bucket/actions/workflows/excavator.yml/badge.svg)](https://github.com/HarjjotSinghh/scoop-bucket/actions/workflows/excavator.yml)

A [Scoop](https://scoop.sh) bucket for Windows apps by Harjot Singh.

| App | Manifest | Install |
| --- | --- | --- |
| [Helicon](https://helicon.sh), a desktop app for the Muse Code CLI | [`bucket/helicon.json`](bucket/helicon.json) | `scoop install helicon/helicon` |
| [Reinstate](https://reinstate.dev) | [`bucket/reinstate.json`](bucket/reinstate.json) | `scoop install helicon/reinstate` |

## Install

```pwsh
scoop bucket add helicon https://github.com/HarjjotSinghh/scoop-bucket
scoop install helicon/helicon
```

The bucket name after `scoop bucket add` is your choice. The commands above use `helicon`.

## Updates

The Excavator workflow runs `checkver` every 4 hours and commits new versions with their hashes, so each manifest
follows its app's GitHub releases. Run `scoop update` and then `scoop update <app>` to pick them up.

Built from [ScoopInstaller/BucketTemplate](https://github.com/ScoopInstaller/BucketTemplate).
