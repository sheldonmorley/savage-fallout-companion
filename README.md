# Savage Fallout Companion

A fan-made **Savage Worlds Adventure Edition (SWADE)** setting companion for the Fallout wasteland, with a Foundry VTT module for online play.

It covers character creation (ancestries like ghouls, super mutants, Gen 3 synths and Mister Handy robots, plus faction Backgrounds), Edges and Hindrances, weapons and mods, armor and full-suit power armor, chems, food and drink, scavenging and crafting at workbenches, radiation as Rad Fatigue, robots and companions, factions, a full bestiary, and a Game Master's section.

## What's here

| File | What it is |
|---|---|
| [`docs/Savage_Fallout_Companion.pdf`](docs/Savage_Fallout_Companion.pdf) | The complete book (about 190 pages) |
| [`docs/Savage_Fallout_Companion_for_Google_Docs.docx`](docs/Savage_Fallout_Companion_for_Google_Docs.docx) | The same book as a Word file you can open in Google Docs |
| [`releases/`](releases/) | Foundry module zips up to 2.9.2. From 2.9.3, which includes the art, each version is a download on the [Releases](https://github.com/sheldonmorley/savage-fallout-companion/releases) page |
| [`module.json`](module.json) | The Foundry install manifest |
| [`CHANGELOG.md`](CHANGELOG.md) | What changed in each version |

## Installing in Foundry VTT

1. In Foundry's setup screen, open **Add-on Modules** and click **Install Module**.
2. Paste this into the **Manifest URL** box at the bottom and click **Install**:

   ```
   https://raw.githubusercontent.com/sheldonmorley/savage-fallout-companion/main/module.json
   ```

3. Enable **Savage Fallout Companion** in your SWADE world.

Foundry will tell you when a new version is out.

**Requires:** Foundry VTT v13 or v14, the SWADE system, and the **SWADE Core Rules** module. The book references the **SWADE Science Fiction Companion** by page.

## In Foundry

- Compendiums for every ancestry, Edge, Hindrance, weapon, armor piece, mod, chem, food item, creature and roll table, plus a journal for every chapter.
- A **Workbench** for crafting and installing mods: double-click a workbench token on the map to open that bench, pick a recipe and craft it from its card, and drag mods onto weapons and armor. Away from a bench, the C.A.M.P. handles cooking and **Break Down Junk** (Junk and unwanted gear into crafting Resources, no roll needed).
- **Automated scavenging:** drop a Scavenge Node token on a map (20 stock locations, from a footlocker to a military depot), put an `@Scavenge[...]` button in a journal, or call it from a tile or region. The player rolls; the GM's client draws the loot cards and adds the items, caps and Junk to their character. See the *12b. Scavenging (Foundry)* journal.
- **Works with The Stockpile** shop module: shops use each character's caps, and Junk and trade goods sell at full value.

## Follow along

Updates, releases and discussion happen in the SWADE Fallout Facebook group:
https://www.facebook.com/share/g/19sfzLopoU/

## Legal

An unofficial fan conversion for personal use. Fallout is a trademark of Bethesda Softworks LLC. Savage Worlds is a trademark of Pinnacle Entertainment Group. This work is not affiliated with or endorsed by either company. You need the Savage Worlds Adventure Edition core rules to play.
