# Changelog

What changed in each version of the book. The version number matches the Foundry module release it shipped with.

## 2.9.5 (November 15, 2026)

- **A new Workbench** (Foundry module only). Each bench opens on its own art, with its own recipes and nothing else, since crafting them needs that bench.
  - **Pick a recipe** from a search box: type part of a name, or open the list. Dots show what's ready (green), short of materials (red), Edge-locked (grey) or rare and unlearned (gold).
  - **The recipe card** shows the item, its ingredients against what the character carries, the result, the roll with its modifiers, the time and any Edge, with **Craft** at the bottom. Click to choose between alternative ingredients (Psycho's Stimpak or Diluted Stimpak). The GM teaches and forgets rare recipes from the card.
  - **Mods by drag and drop** on the Weapons Workbench, Armor Workbench and Power Armor Station: pick an item, then drag a mod onto its slot, or drag it back off to take it out (each still a Repair roll). Power armor shows its Mod slots as a meter. The Robot Workbench keeps its robot and Automatron panel, restyled.
  - **The C.A.M.P.** replaces the no-station view: cooking and Break Down Junk anywhere, plus mods at −2 with a Deluxe Toolkit.
  - New bench art for all six benches and the C.A.M.P. See *12a. Workbench (Foundry Crafting)*.

## 2.9.4 (November 15, 2026)

- **The Workbench shows current item art** (Foundry module only). It read each recipe's picture from a copy saved when the recipe list was made, so 154 recipes showed old or missing art after the items were updated. It now reads the art from the compendiums when it opens, including add-on recipes, so new art shows up there automatically.

## 2.9.3 (November 15, 2026)

- **The art ships with the module** (Foundry module only). Item art, adversary art and tokens, scene maps, tiles, skill icons and the radio and weapon audio are now in the download, so installing or updating from the manifest gives you everything, not just the rules. The download is about 200 MB and is published as a GitHub Release.
- **Three adversary tokens fixed** (Foundry module only): the Assaultron, Bloodbug and Eyebot pointed at token files with the wrong capitalization, which broke them on The Forge and other Linux hosts.

## 2.9.2 (November 15, 2026)

- **Breaking Down Junk needs no roll.** With a workbench, a Toolkit, or a Multi-Tool, every 10 caps of Junk gives 5 Common and 1 Uncommon Resources in 30 minutes; a last part of 10 caps gives its share, rounded down. The Repair roll, its results table, the −2 for working without tools, and Tech Junk are gone. A new table in the rule shows what each hero gets, and a note explains when to sell Junk instead.
- **New Edges: Scrapper and Improved Scrapper** (Converted Perks). A Scrapper (Novice, Repair d6+) gets an extra Uncommon per 10 caps of Junk, in half the time. Improved Scrapper (Seasoned, Scrapper) adds a Rare per 20 caps. Both are in the Edge Summary and the Edges compendium.
- **Break Down Junk in the Workbench** (Foundry module only). A button in the Workbench, a *Break Down Junk* macro, and `SavageFallout.breakDownJunk()`: choose how much Junk to break down and any unwanted weapons, armor or gear to scrap at half price, and the Resources go on the sheet with Scrapper and Improved Scrapper applied. Worn gear, consumables, ammo, fusion cores and trade goods aren't offered. See *12a. Workbench (Foundry Crafting)*.

## 2.9.1 (November 15, 2026)

- **Scavenger Edge:** on a raise, a Scavenger now draws one extra loot card, which ignores the location's Max Loot Cards, instead of two cards for every card. The salvage is still doubled. The Edge and the Scavenging rules now say the same thing, and the Edge points to the right chapter.
- **The book sticks to play at the table.** The PDF and Word file leave out notes that only apply in Foundry: the Foundry column of the chem Effect Vocabulary table, "in Foundry, roll the table" asides, and Foundry-only changelog entries. The module's journals keep them.
- **Junk and trade goods sell at full value in The Stockpile** (Foundry module only), as Selling Salvage says, whatever the shop's usual buy-back rate.
- **The Stockpile uses caps** (Foundry module only): if its wallet field and currency name aren't set, the Companion sets them to each character's caps.

## 2.9.0 (November 15, 2026)

- **Automated scavenging** (Foundry module only). Every search in the Scavenging rules can now run itself: the player makes the Notice or Survival roll, and the GM's client draws the loot cards, reads them on the Scavenging Loot tables, and adds the items, caps and Junk to the character. Degree, Tier, Scale, repeat searches, Scavenger, Scrounger, Investigator, Jokers, Complications and locked containers all follow the chapter. See the new *12b. Scavenging (Foundry)* journal.
- **Three ways to place a search:** Scavenge Node tokens (a new compendium with 20 stock locations, from a footlocker to a military depot), a script for Monk's Active Tiles or Regions, and `@Scavenge[...]` buttons in journals. Any location can read its loot from a roll table instead, such as the Winter Wasteland table.
- **New items:** Junk (tracked by its value in caps, 1 cap and 1 lb per unit) and four trade goods named in the loot tables: Locket, Silver Pocketwatch, Pre-War Money and Pre-War Valuables.
- **New macros:** *Restock Scavenging (This Scene)* and *Scavenge Here*.
- **New setting:** Whisper scavenging results to the GM and the searching player.

## 2.8.4 (October 19, 2026)

- Foundry module only: the Workbench remembers the last character token you selected, so clicking a workbench token on the map no longer loses your crafter. As GM with no player-owned characters, you can pick any character to craft with.

## 2.8.3 (October 19, 2026)

- Foundry module only: the Rad Resistant Edge's +2 now applies only to radiation Vigor rolls (it's offered in the roll dialog), not to every Vigor roll. Add-on weapons can now refuse generic mods, so the Workbench offers only the mods each weapon can take.

## 2.8.2 (October 16, 2026)

- **Ghouls:** Repugnant is replaced by Outsider (Minor): −2 to Persuasion with anyone who isn't a ghoul, except in ghoul communities and tolerant towns like Goodneighbor. It's the standard SWADE Hindrance, worth the same −1, so the ghoul still totals +2.

## 2.8.1 (October 16, 2026)

- **Chosen of Atom:** Atom's Shield now reduces penalties from Rad Fatigue by 1, instead of ignoring only the first level's penalty. It keeps helping as the Glow builds up. The levels still count on the Fatigue track and toward the Breaking Point.
- **Layout fix:** 29 bulleted lists in the PDF, such as Chosen of Atom's abilities, ran together into the paragraph before them. They now display as lists.

## 2.8.0 (October 13, 2026)

- **Prices follow the 2d20 game.** Every item with a Fallout 2d20 equivalent now costs what the 2d20 core rulebook charges: 199 items in all, mostly mods, chems, food, clothing, and armor. Items invented for Savage Fallout keep their prices.
- **Power armor** costs the full 2d20 suit total: frame plus pieces, from 4,950 caps (Raider) to 5,720 (X-01).
- **Arms and Legs** pieces and their mods cost double the 2d20 single-limb price, because they come as pairs.
- **Mods that 2d20 prices per weapon** use the middle of those prices.
- **Mod tier tables** in Weapons and Armor are now the price guide for mods you design yourself; the listed mods use their 2d20 prices.
- **Background kits** keep their value: loose caps changed for Brotherhood of Steel (80), Chem Runner (25), Cultist (35), Feral (132), Railroad Operative (60), Raider (105), and Tribal Outsider (117). Starting Funds stay at 100 caps.
- **Game Master's Section:** the advice on pricing 2d20 gear was rewritten to match.

## 2.7 (October 8–10, 2026)

- **Adventures removed.** The book no longer points to adventures packaged with the Foundry module; those are now separate modules.
- **Vehicle skills:** the last reference to Piloting (in the Game Master's Section) now uses Electronics.
- **Vault Dweller** no longer grants a free Vault Jumpsuit or Pip-Boy anywhere.
- Foundry module only: compendium folders, art and icon fixes, a single dependency on SWADE Core Rules, and sheet layout fixes.

## 2.6 (October 7, 2026)

- **Crafting stations.** Every recipe except cooking needs its workbench; there is no field crafting. A Deluxe Toolkit lets you repair and install mods away from a bench at −2.
- **Backgrounds rebalanced:** four Edges each, at most one powerful pick, and a starting kit worth about 200 caps with a weapon and an outfit.
- **Faction Edges removed.** Faction identity comes from the faction Backgrounds; joining a faction in play uses Connections or Soldier.
- **Armor Arms and Legs are pairs,** covering both limbs.
- **Vehicle skills removed:** no Boating, Driving, Piloting, or Riding, and no Edges that depend on them.
- **Robot mods added** from the 2d20 book.
- **Spikers removed** (Hand Spiker and Longarm Spiker). The Raider starts with a Pipe Revolver and the Wanderer with a Pipe Bolt-Action.
- **Skill books** renamed: Lying, Congressional Style and Total Hack.

## Earlier October 2026

- **Radiation is Rad Fatigue.** Radiation uses the normal Fatigue track instead of a separate Rad count, and doesn't recover with rest. RadAway removes a level.
- **Power armor is full suits** on the Science Fiction Companion framework, with slot-based mods and the Excavator, Ultracite, Hellfire, and Advanced Mk II added.
- **First complete edition** of the book: all seventeen chapters, from character creation to the Game Master's Section.
