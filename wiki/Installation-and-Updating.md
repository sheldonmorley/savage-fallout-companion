# Installation and Updating

## Requirements

- **Foundry VTT** v13 or v14.
- **Savage Worlds Adventure Edition** game system (5.0 or later; tested on 6.0.3).
- **SWADE Core Rules** module (Pinnacle's official module). Foundry asks for it when you install.

Optional, and never required:
- **The Stockpile**: the Companion makes it use each character's caps and sell Junk and trade goods at full value.
- **Monk's Active Tiles**: one of three ways to trigger a scavenging search (see [[Scavenging]]).

## Installing

1. In Foundry's setup screen, open **Add-on Modules > Install Module**.
2. Paste this into **Manifest URL** and click **Install**:
   ```
   https://raw.githubusercontent.com/sheldonmorley/savage-fallout-companion/main/module.json
   ```
3. Launch your SWADE world, open **Manage Modules**, and enable **Savage Fallout: Fallout Companion** (and SWADE Core Rules).

The download is about 200 MB, because all the art, tokens, scenes and audio ship with the module.

The first time a GM loads the module in a world, SWADE's core skill settings are pointed at the Fallout skills, so new characters start with the Fallout versions of Athletics, Common Knowledge, Notice, Persuasion and Stealth. This happens once; you can change it afterwards in the SWADE settings.

## Updating

Foundry checks the manifest for you: **Add-on Modules > Update** (or **Check for Updates**). GitHub can take a few minutes to show a new version after it's released, so if Foundry still offers the old one, wait and check again.

## Where things live

| | |
|---|---|
| Module page | https://github.com/sheldonmorley/savage-fallout-companion |
| Releases (zips) | https://github.com/sheldonmorley/savage-fallout-companion/releases |
| Book (PDF and Google Docs) | https://github.com/sheldonmorley/savage-fallout-companion/tree/main/docs |
| What changed | [CHANGELOG.md](https://github.com/sheldonmorley/savage-fallout-companion/blob/main/CHANGELOG.md) |

If an update fails with a "permission denied" (EACCES) error, see [[Troubleshooting and FAQ]].
