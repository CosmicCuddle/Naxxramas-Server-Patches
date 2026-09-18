# Naxxramas Server Patches

Client patch documentation and downloads for the **Naxxramas World of Warcraft 3.3.5a server**.

This repository keeps a permanent record of the client patches used by Naxxramas, including required Main Server Patches and separate Optional Patches.

## Downloads

### Required Main Server Patch
➡️ [Download the latest Naxxramas Main Server Patch](https://github.com/CosmicCuddle/Naxxramas-Server-Patches/releases/tag/v1.0.6.8.2)

Required to play on the Naxxramas server.

### Optional Client Patches
➡️ [View the Naxxramas Optional Client Patches](https://github.com/CosmicCuddle/Naxxramas-Server-Patches/releases/tag/optional-v1.0)

Includes the Vanilla and Burning Crusade login/loading screen replacements.

## Current Main Server Patch

**Version 1.0.6.8.2**

The required client patch set currently consists of:

- `patch-V.mpq`
- `patch-Z.mpq`

The MPQ files are distributed through GitHub Releases rather than being committed directly to the repository.

## Patch Categories

### Main Server Patches

These patches are required for the Naxxramas client to correctly support server-side changes, custom data and Individual Progression integration.

See **[PATCHES.md](PATCHES.md)** for the reconstructed Main Server Patch history from Patch 1.0.1 onward.

### Optional Patches

Optional patches are separate client modifications that are not required to connect to or play on the server.

See **[OPTIONAL-PATCHES.md](OPTIONAL-PATCHES.md)**. This section will be expanded as the optional patch collection is documented.

## Installation

1. Download the latest required Main Server Patch files from the repository's **Releases** section.
2. Close World of Warcraft before replacing patch files.
3. Place the required `.mpq` files in your World of Warcraft 3.3.5a `Data` folder.
4. Replace older versions of the same Naxxramas patch files when updating.
5. If the release notes, Discord announcement, or in-game server restart message tells you to refresh your client cache, delete the `Cache` folder before starting the game again.
6. The `Cache` folder is found in your main World of Warcraft 3.3.5a installation folder, usually alongside folders such as `Data`, `Interface` and `WTF`.
7. Start World of Warcraft normally. The client will automatically rebuild the `Cache` folder when needed.

Always use the patch files from the latest Naxxramas Main Server Patch release and follow any additional instructions included in the release notes, server announcements or in-game restart messages.

## Compatibility

These patches are built specifically for the **Naxxramas** server and its customised **AzerothCore 3.3.5a** setup, including **Individual Progression** integration.

They should not be treated as general-purpose AzerothCore or World of Warcraft patches.

## Patch History

The Main Server Patch history has been reconstructed from the archived MPQ releases, DBC files, saved working data and Individual Progression update resources. Where working files were present but never included in the finished MPQ, they are recorded as development history rather than released changes.

See **[PATCHES.md](PATCHES.md)** for the full history.

## Credits

Maintained by **CosmicCuddle** for the Naxxramas server.

World of Warcraft and related names, artwork and assets are trademarks or copyrights of Blizzard Entertainment. This project is not affiliated with or endorsed by Blizzard Entertainment.
