# Blazing:Rebirth versions

Generated from [`versions.json`](versions.json) by `source/tools/publisher/release_manager.py`. Launchers check their channel's signed feed; see the [README](README.md).

## Channels

| Channel | Launcher | Version name | Release | Content | Feed signed |
| --- | --- | --- | --- | --- | --- |
| stable | none yet | | | | |
| beta | 35 | 0.25-tutorial-rc | [launcher-v35-beta](https://github.com/notgate/blazing-rebirth-cache/releases/tag/launcher-v35-beta) | 2 | 2026-09-28 |

## Launcher builds

| Launcher | Version name | Runtime | Content | Channels | x86_64 SHA-256 | arm64-v8a SHA-256 |
| --- | --- | --- | --- | --- | --- | --- |
| 35 | 0.25-tutorial-rc | 121 | 2 | beta | `7734e30aa3e2fbf4…` | `e0135a546244681e…` |
| 34 | 0.24.3-history-rc | 121 | 2 | beta | `64b1e3ae2c714e1a…` | `8f65730bfa6bb248…` |
| 33 | 0.24.2-history-rc | 121 | 2 | beta | `d5e9ea80c9d50fd5…` | `6612f3734185886b…` |
| 31 | 0.24.1-history-rc | 121 | 2 | beta | `4066d453b5552791…` | `71583ca8f4d453c4…` |
| 30 | 0.24-history-rc | 121 | 2 | beta | `89f19c26aff23538…` | `4c5b82e88706e364…` |
| 29 | 0.23-channels-rc | 121 | 2 | beta | `d6088fd0af5d015d…` | `6bfac607783b7f4a…` |
| 27 | 0.22-channels-rc | 121 | 2 | beta | `caa706d117203fa7…` | `2173452c46194aa9…` |

## Rollback builds

A rollback build is an older launcher repackaged with a higher installer version, so launchers can revert to it without uninstalling (Updates → Release history → Revert). It keeps that launcher's runtime and game data.

| Launcher | Restores | Version name | Runtime | Content | Release | Feed | x86_64 SHA-256 | arm64-v8a SHA-256 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 32 | 30 | 0.24-history-rc | 121 | 2 | [launcher-v32-rollback](https://github.com/notgate/blazing-rebirth-cache/releases/tag/launcher-v32-rollback) | `rollback-30-<abi>.json` | `5d50aebaf3b4ee14…` | `e0b4861f4b0e6272…` |

## Game data caches

| Content | Release | Archive | Size | Parts | SHA-256 |
| --- | --- | --- | --- | --- | --- |
| 2 | [cache-v2](https://github.com/notgate/blazing-rebirth-cache/releases/tag/cache-v2) | Blazing-Rebirth-Data-v2.zip | 3.96 GB | 2 | `816cbde1e2f759d7…` |
| 1 | [cache-v1](https://github.com/notgate/blazing-rebirth-cache/releases/tag/cache-v1) | Blazing-Rebirth-Data-v1.zip | 3.37 GB | 2 | `65f17d2053d53e2f…` |
