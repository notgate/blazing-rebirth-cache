# Blazing:Rebirth versions

Generated from [`versions.json`](versions.json) by `source/tools/publisher/release_manager.py`. Launchers check their channel's signed feed; see the [README](README.md).

## Channels

| Channel | Launcher | Version name | Release | Content | Feed signed |
| --- | --- | --- | --- | --- | --- |
| stable | 42 | 0.29-auto-loop | [launcher-v42](https://github.com/notgate/blazing-rebirth-cache/releases/tag/launcher-v42) | 2 | 2026-10-11 |
| beta | 42 | 0.29-auto-loop | [launcher-v42-beta](https://github.com/notgate/blazing-rebirth-cache/releases/tag/launcher-v42-beta) | 2 | 2026-10-11 |

## Launcher builds

| Launcher | Version name | Runtime | Content | Channels | x86_64 SHA-256 | arm64-v8a SHA-256 |
| --- | --- | --- | --- | --- | --- | --- |
| 42 | 0.29-auto-loop | 172 | 2 | beta, stable | `0d8a534c1d52ab4e…` | `0d97594647d4d040…` |
| 41 | 0.28.1-teams-rc | 124 | 2 | beta | `5f32e89e5cf832aa…` | `bf55a777b423cf2a…` |
| 40 | 0.28-teams-rc | 124 | 2 | beta | `5e5b9461198f7a7b…` | `47ffa4c734cd295f…` |
| 39 | 0.27.1-grind-rc | 122 | 2 | beta, stable | `1c343f80643f19ea…` | `7c57638fb4e61283…` |
| 38 | 0.27-grind-rc | 122 | 2 | beta | `1bb61e23271f93d9…` | `394c0f8091871d29…` |
| 37 | 0.26.1-news-rc | 121 | 2 | beta | `029ec0dd6e7edde5…` | `3dcd3ef3c1d75ec9…` |
| 36 | 0.26-news-rc | 121 | 2 | beta | `6efbed2323afcb74…` | `21a375bc09a32336…` |
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

## iOS (one channel)

The iPhone app checks the signed feed [`ios-updates/update-ios.json`](https://github.com/notgate/blazing-rebirth-cache/releases/tag/ios-updates) itself.

| Release | App build | Data version | Rollback of | Notes |
| --- | --- | --- | --- | --- |
| 5 | [5](https://github.com/notgate/blazing-rebirth-cache/releases/tag/ios-app-v5) | [2](https://github.com/notgate/blazing-rebirth-cache/releases/tag/ios-data-v2) |  | iOS build 5 fixes Fill Ramen on the active Enhance page, spaces Auto Awaken like |
| 4 | [4](https://github.com/notgate/blazing-rebirth-cache/releases/tag/ios-app-v4) | [2](https://github.com/notgate/blazing-rebirth-cache/releases/tag/ios-data-v2) |  | iOS fixes: remove stray unit-tab symbols and update selection on the first tap;  |
| 3 | [3](https://github.com/notgate/blazing-rebirth-cache/releases/tag/ios-app-v3) | [2](https://github.com/notgate/blazing-rebirth-cache/releases/tag/ios-data-v2) |  | Fix iOS crash when entering from the title screen; correct Unit Navigation hook  |
| 2 | [2](https://github.com/notgate/blazing-rebirth-cache/releases/tag/ios-app-v2) | [2](https://github.com/notgate/blazing-rebirth-cache/releases/tag/ios-data-v2) |  | Auto Loop for completed missions: skip scenes, claim rewards, restart continuous |
| 1 | [1](https://github.com/notgate/blazing-rebirth-cache/releases/tag/ios-app-v1) | [1](https://github.com/notgate/blazing-rebirth-cache/releases/tag/ios-data-v1) |  | First iOS offline release: the app downloads its data from GitHub and updates it |

## Game data caches

| Content | Release | Archive | Size | Parts | SHA-256 |
| --- | --- | --- | --- | --- | --- |
| 2 | [cache-v2](https://github.com/notgate/blazing-rebirth-cache/releases/tag/cache-v2) | Blazing-Rebirth-Data-v2.zip | 3.96 GB | 2 | `816cbde1e2f759d7…` |
| 1 | [cache-v1](https://github.com/notgate/blazing-rebirth-cache/releases/tag/cache-v1) | Blazing-Rebirth-Data-v1.zip | 3.37 GB | 2 | `65f17d2053d53e2f…` |
