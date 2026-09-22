# Blazing:Rebirth cache hosting

Public release-asset storage for the checksum-pinned Blazing:Rebirth cache. Download payloads are attached to [Releases](https://github.com/notgate/blazing-rebirth-cache/releases), not committed into Git or stored in Git LFS.

## Cache v1

The original ZIP is split into two raw byte segments, each below GitHub's 2 GiB per-asset limit. Concatenating `.part01` followed by `.part02` restores the exact original ZIP; per-part and whole-archive hashes are in `cache-v1.json`.

The cache contains no player saves, session credentials or personal accounts. Installer integration is in progress. Installer 17 cannot consume these split assets; an individual part is not a valid full-ZIP mirror.

Publishing cache bytes does not qualify an installer or native game for release. Gameplay, device support and updater approval are separate.

This is an unofficial community project and is not affiliated with the original game's publishers. Original assets remain subject to their owners' rights; this repository grants no additional license to them.
