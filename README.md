# Blazing:Rebirth releases and game data

Public release assets for Blazing:Rebirth: the checksum-pinned game-data caches and the signed launcher update channels. No source code, saves, credentials or keys are stored here. Payloads are [release](https://github.com/notgate/blazing-rebirth-cache/releases) assets, never Git or LFS files.

## Versions

[`versions.json`](versions.json) is the version registry; [`VERSIONS.md`](VERSIONS.md) is its readable view. It lists which launcher build each channel serves, every published launcher build with its APK hashes, and every game-data cache with its parts. It is written only by `release_manager.py` after the release assets were uploaded and verified.

## Launcher update channels

| Channel | Who gets it | Feed release | Launcher releases |
| --- | --- | --- | --- |
| Beta | Testers who pick Beta in the launcher (Updates, Channel) | [`apk-updates-beta`](https://github.com/notgate/blazing-rebirth-cache/releases/tag/apk-updates-beta) | `launcher-v<N>-beta` (pre-releases) |
| Stable | Everyone else (default) | [`apk-updates`](https://github.com/notgate/blazing-rebirth-cache/releases/tag/apk-updates) | `launcher-v<N>` |

Each feed holds one signed manifest per Android ABI (`update-x86_64.json`, `update-arm64-v8a.json`). Installed launchers check their channel automatically when idle and online. They accept an update only when:

- the manifest's P-256 signature matches the key built into the launcher, it has not expired, and its sequence is newer than any manifest the phone has already seen;
- it is for the phone's ABI and channel, raises the installer version, and never lowers the runtime or content version;
- the GitHub release is published in that channel and its APK asset has the signed size and SHA-256. The downloaded APK is checked again, including its package, signer and embedded versions, before Android's installer opens.

Builds reach Stable only after they were published to Beta.

Update checks need launcher 29 or later on Android 9 and 10 (earlier launchers switched them off there, "archive-signer"); install 29 once by hand on such phones. Android 11 and later can update from launcher 27.

## Game data caches

Each cache is a ZIP split into raw byte segments below GitHub's 2 GiB asset limit. Joining `.part01`, `.part02`, … in order restores the exact archive; `cache-v<N>.json` pins every part and the whole archive by size and SHA-256. The content version is the `N` in `cache-v<N>`.

A launcher pins exactly one cache. A launcher update that moves to a new content version tells the player that new game data follows; after installing, the launcher shows "Needs game data" and downloads the new cache once (saves are kept). The cache is always published before any launcher that pins it.

## Disclaimer

This is an unofficial community project and is not affiliated with the original game's publishers. Original assets remain subject to their owners' rights; this repository grants no additional license to them.
