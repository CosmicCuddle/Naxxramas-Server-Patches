# Optional Naxxramas Client Patches

These patches are completely optional. They are not required to connect to or play on the Naxxramas server and are kept separate from the required Main Server Patch files.

The optional patches currently available are visual client replacements for the World of Warcraft 3.3.5a login and loading screens.

## Patch-J — Vanilla Login Screen

`patch-J.mpq` restores a Vanilla-style login screen while using the Wrath of the Lich King 3.3.5a client.

### Changes

- Replaces the Wrath login-screen model and associated textures with the Vanilla-style login screen.
- Replaces the Wrath login-screen music with the music bundled in the patch.
- Contains several additional Vanilla-style loading-screen assets used by the package.

### Installation

Place `patch-J.mpq` in your World of Warcraft 3.3.5a `Data` folder and restart the client.

Do not use `patch-J.mpq` and `patch-C.mpq` together because both replace the same login-screen files.

---

## Patch-U — Vanilla Loading Screens

`patch-U.mpq` restores Vanilla-style loading screens for the original two continents.

### Changes

- Replaces the Eastern Kingdoms loading screen.
- Replaces the Kalimdor loading screen.
- Includes both standard and widescreen versions of those loading screens.

This patch only changes loading-screen artwork and does not make any server-side changes.

### Installation

Place `patch-U.mpq` in your World of Warcraft 3.3.5a `Data` folder and restart the client.

`patch-U.mpq` can be used alongside a login-screen patch. It is intended to complement `patch-J.mpq` when using the Vanilla-themed client appearance.

### Credit

HD Vanilla loading-screen artwork credited to **slendydaddy**.

---

## Patch-C — The Burning Crusade Login Screen

`patch-C.mpq` replaces the Wrath of the Lich King login screen with a Burning Crusade-style Dark Portal login screen.

### Changes

- Replaces the Wrath login-screen model and associated textures with the Burning Crusade-style Dark Portal screen.
- Includes the Dark Portal, Hellfire and related visual assets used by the replacement screen.
- Replaces the Wrath login-screen music with the music bundled in the patch.

### Installation

Place `patch-C.mpq` in your World of Warcraft 3.3.5a `Data` folder and restart the client.

Do not use `patch-C.mpq` and `patch-J.mpq` together because both replace the same login-screen files.

---

## Removing an Optional Patch

Close World of Warcraft and remove the relevant optional `.mpq` file from the `Data` folder. The client will then return to the files supplied by the normal 3.3.5a client or another higher-priority patch.

These optional files are independent from the required Naxxramas Main Server Patch. Do not remove `patch-V.mpq` or `patch-Z.mpq` when changing optional patches.
