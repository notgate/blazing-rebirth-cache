# Blazing:Rebirth cache hosting

Public release-asset storage for the checksum-pinned Blazing:Rebirth cache. Download payloads are attached to [Releases](https://github.com/notgate/blazing-rebirth-cache/releases), not committed into Git or stored in Git LFS.

## Cache v1

The original ZIP is split into two raw byte segments, each below GitHub's 2 GiB per-asset limit. Concatenating `.part01` followed by `.part02` restores the exact original ZIP; per-part and whole-archive hashes are in `cache-v1.json`.

Installer 18 downloads both parts automatically, resumes paused transfers, verifies each part and the complete ZIP, then imports the cache through its existing member-integrity checks. GitHub is the primary cache source; the existing Drive endpoint and configured complete-ZIP mirrors remain fallbacks. Testers do not need a GitHub account or token, and do not need to join files manually.

The cache contains no player saves, session credentials or personal accounts. Installer 17 cannot consume these split assets; an individual part is not a valid full-ZIP mirror.

The exact installer 18 x86-64 test APK completed a full public GitHub download, pause/resume, reassembly and verification/import of all 6178 files on BlueStacks. That isolated test used an opaque, GitHub-only TLS proxy to retain the emulator's nonloopback firewall blocks; the APK contains no test proxy configuration. The ARM64 APK was built and package-verified, but this generation has not been rerun on physical ARM hardware. Installer APKs are distributed separately as test candidates, not attached to this cache release. Install them manually: the tested native Settings screen reports that update verification is unavailable, so native OTA updating is not qualified.

Publishing cache bytes does not qualify an installer or native game for release. Gameplay, device support and updater approval are separate.

This is an unofficial community project and is not affiliated with the original game's publishers. Original assets remain subject to their owners' rights; this repository grants no additional license to them.
