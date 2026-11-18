# Changelog

What changed in each version of the book. The version number matches the Foundry module release it shipped with.

## 2.13.0 (November 18, 2026)

- **Weapons line up with SWADE.** Where a weapon has a SWADE or Science Fiction Companion counterpart, it now uses those stats. The **Combat Shotgun** is drum-fed like SWADE's Streetsweeper: 12 shots, Min Str d6, 10 lbs. The **Combat Knife** is Str+d4, like SWADE's survival knife.
- **Inaccurate is gone.** It wasn't a SWADE quality. The Submachine Gun, Gamma Gun and Institute Laser lose it.
- **Weapon mods that removed Inaccurate do something else:** Comfort Grip, +1 Shooting at Short Range; Full Stock, +1 Shooting at Medium Range; Marksman's Stock, +1 Shooting at Long Range; Sharpshooter's Grip, +1 Shooting when Aiming; Compensator, −2 Recoil; Gyro-Compensating Lens, ignore 2 points of Range penalties when Aiming. The Automatic Receiver's drawback is now Range −1 step.
- **Two Hands is for melee weapons only**, as in SWADE: one-handed use is at −4 and loses Reach and Parry bonuses, but the wielder keeps full Strength for damage. The **Spear** gets Parry +1 only when used two-handed, and the **Pool Cue** gains Parry +1. Guns no longer carry it.
- **Edges look at a gun's type, not its hands.** Weapon Specialist (Gunslinger) covers pistols and Weapon Specialist (Rifleman) covers rifles and shotguns; Sniper works with any rifle.
- **Stocks turn pistols into rifles.** A Full Stock, Marksman's Stock or Recoil-Compensating Stock makes a pistol count as a rifle (it loses Concealed). A Sawed-Off Barrel makes a shotgun count as a pistol.
- **Fewer weapon qualities.** Rules that only one weapon used are now written into that weapon's description: the Laser Musket's cranking, the Junk Jet's ammunition, the Tesla Rifle's arcing bolt, mines, and the Pulse grenade and mine. Arcing, Crank, Dart, Junk, Mine, Pulse, Recon and Revolver are no longer qualities. Mountable is now **Mounted Weapon**, as in the Science Fiction Companion. Revolvers still can't take Magazine mods.
- **Mines** work as in the Science Fiction Companion: setting one takes an action, it goes off when triggered by weight, impact or its sensors, and spotting a well-hidden mine is a Notice roll at −4.
- **Accurate and Suppressed come only from mods.** The Hunting Bow, Crossbow, Throwing Knife, Tomahawk and Syringer are no longer Suppressed; the 10mm Pistol, Silenced and the Deliverer keep their built-in suppressors. The **Recon Scope** marks your Aimed target itself: the first ally to attack it before your next turn adds +1.
- **In Foundry** (module only):
  - Every weapon item uses one entry format: type and skill, a short description, the stats, Notes, Special rules, the Mods it takes (worked out from the module's own mod data) and how it is built and repaired, with the qualities it uses defined underneath.
  - The Weapons chapter journal gives every weapon the same entry under its table, and lists Breaker (the Sledgehammer and Super Sledge now use it) among the qualities. A design note explains that energy weapons follow Savage Fallout's own progression rather than SWADE's laser tables.
  - Weapon items spell out the rules that used to be qualities in their Special line, and their Weapon Qualities glossary lists only real qualities. Mod items that granted or removed Two Hands, Recon or Mountable are updated, and the stocks note that they make a pistol count as a rifle.
  - **Junk is a consumable** now, like the other ammunition, and it is the Junk Jet's ammo. Salvaging, scavenging, the stockpile and the workbench still find it by name.
  - Adversaries and the Mister Handy carry the updated weapons.

## 2.12.2 (November 17, 2026)

- **Pip-Boy map pins show up again** (Foundry module only). Foundry's own styling shrank the pin icons to nothing, so pins were on the map but invisible. Fixed.
- The Pip-Boy map now reads scene backgrounds the Foundry 14 way (from the scene's level), so it won't break when Foundry drops the old way, and it places pins correctly on scenes with padding or an offset background. Pins it has to skip are now noted in the browser console with the reason.

## 2.12.1 (November 17, 2026)

- **The Pip-Boy's STATUS page gets a figure** (Foundry module only). It shows the character's own portrait, tinted green; full-body portraits look best, and characters still on a stock icon get an outline figure. Around it, six readouts show the armor worn on the head, arms, torso and legs: the best equipped piece and its bonus, with every piece listed when you hover. They update as gear is equipped or removed.

## 2.12.0 (November 16, 2026)

- **Radiation is now rads.** A failed radiation roll gives a **rad**, marked in a Wound box from the far end of the track. Rads give no penalty, but each one leaves room for one less Wound. Rest, healing and Stimpaks never remove them; RadAway and the other treatments do. This replaces Rad Fatigue, which shared the Fatigue track, made each later roll harder, and stacked with hunger and heat.
- **Radiation Sickness:** a rad that fills a box past the end of the track leaves the hero Incapacitated (not Bleeding Out) until treated. Each day untreated, a Vigor roll; failure means a Breaking Point roll, and a Critical Failure is fatal.
- **Breaking Point** now comes at 2 rads, with another roll for each rad after that.
- **Extras** take each rad as a level of Fatigue that rest doesn't remove, and never reach the Breaking Point.
- **Irradiated food and water:** the daily Vigor roll is now at +1 (0 if you had a lot).
- **Chosen of Atom:** your first rad takes up no Wound box (it still counts for the Breaking Point). **Rad Intolerant:** a failure gives 2 rads (3 on a Critical Failure).
- Every Edge, Hindrance, ancestry, food, chem, weapon, robot mod and bestiary entry now says rads.
- **In Foundry** (module only):
  - Wild Cards keep a rad count and a *Rads* effect that lowers their maximum Wounds, so SWADE's own Incapacitation still works. Reaching 2 rads, and each rad after, posts a Breaking Point reminder; overflowing the track applies Radiation Sickness.
  - The standard SWADE sheet gets a **Rads** counter beside Wounds, with + and − buttons.
  - The Pip-Boy shows rads as red boxes on the Wounds row, with a Rads row to set them.
  - RadAway, Diluted RadAway, Brahmin Milk, Mutant Hound Chops and the Refreshing Beverage remove rads when used.
  - On first load, the GM's client turns each character's marked Rad Fatigue from 2.11 or earlier into rads.
  - Macros: `SavageFallout.addRads`, `removeRad`, `setRads` and `radsOf`.

## 2.11.1 (November 16, 2026)

- **The Pip-Boy shows every item's own art** (Foundry module only), tinted green, at the top of its detail panel: mods, recipes and gear that had no picture now have one, and it's always the current art. Pictures copied into item descriptions are no longer shown there.
- Orange Mentats' description showed the plain Mentats picture; fixed.

## 2.11.0 (November 16, 2026)

- **Crafting Edges no longer grant a free schematic or a signature mod.** Taking the Edge already teaches all of its recipes, so the extra schematic did nothing. Gun Nut, Armorer, Blacksmith, Science! and the three Improved Edges are updated in the book, the Edges and the journals.
- **Science! Masterwork recipes are Rare** (12 of them: Six-Crank Capacitor, Electrified Serrated Blade, Stun Pack, BioCommMesh, Nanofilament, Shielded Lining, Core Assembly, Jetpack, Tesla Bracers, and the Nuka, Plasma and Pulse Grenades). They must be found or taught.
- **Found recipes are items** (Foundry module only). All 28 rare recipes are in *Fallout Crafting Materials > Rare Recipes* as *Formula:*, *Recipe:* and *Schematic:* items. Using one teaches the recipe to that character and uses it up; if they already know it or lack its Edge, nothing is used up. On the Pip-Boy they're under ITEMS > MISC with a Learn button.
- **Mr. Fix It** is just SWADE's Edge again: +2 to Repair rolls, and a raise halves the time. It no longer mentions recipes of its own (there were none).
- **Improved Scrapper** now also needs Repair d8+, like the other Improved crafting Edges.
- **The Pip-Boy gets MAP and RADIO** (Foundry module only), on the DATA tab.
  - **MAP:** WORLD shows a scene the GM picks in the settings (the Companion ships no map, so each campaign uses its own); LOCAL shows the scene you're on. Drag to pan, scroll to zoom, and your token shows where you are. The scene's map pins are the markers: a pin's journal entry at Limited shows an undiscovered outline, at Observer the found icon with an Open button, so the GM reveals locations by raising permissions.
  - **62 Pip-Boy location icons** (with found and undiscovered versions), plus quest destination, signal source and location pins, join Foundry's map-pin icon list. Icons by the League of Raconteur Explorers, used under licence.
  - **RADIO:** the Companion's Fallout Radio and any playlists in a world folder named *Radio*. Tuning in plays on your computer only, shuffled, with its own volume, and keeps going with the Pip-Boy closed. Players can't play to the table; the GM can, as an ordinary playlist.
  - See *02a. Pip-Boy Sheet (Foundry)*.

## 2.10.0 (November 15, 2026)

- **A Pip-Boy character sheet** (Foundry module only). Open a character's sheet settings and choose *Pip-Boy*, or run `SavageFallout.openPipBoy()`. It reads the character live:
  - **STATS:** Wounds, Fatigue and Rad Fatigue as clickable boxes, conditions, active effects with their time left, and Pace, Parry, Toughness and Bennies; attributes and skills to roll; Edges, Hindrances and abilities.
  - **ITEMS:** Weapons, Apparel, Aid, Misc and Ammo, with weight against the load limit. Attack, Equip, Use (chems and food apply their effects) and Open.
  - **DATA:** Quests and Notes from shared journals in the folders named *Quests* and *Notes*; a *Completed* subfolder marks quests done.
  - The three knobs switch tabs, the left dial steps through sub-tabs (click or scroll), the rad gauge follows Rad Fatigue, and the controls make Pip-Boy sounds. It scales with the window. Clear the frame setting for a plain screen instead.
  - Frame art by ABBSTractGraphics, used with permission. See *02a. Pip-Boy Sheet (Foundry)*.
- **Rad Fatigue is marked** (Foundry module only). The character keeps a count of how many Fatigue levels came from radiation, as the Radiation rules ask; the Pip-Boy sheet shows and sets it, and RadAway (and Diluted RadAway) now clear a marked level.

## 2.9.6 (November 15, 2026)

- **Fixed the Workbench's title bar** (Foundry module only): its close and other buttons showed empty boxes instead of their icons.

## 2.9.5 (November 15, 2026)

- **A new Workbench** (Foundry module only). Each bench opens on its own art, with its own recipes and nothing else, since crafting them needs that bench.
  - **Pick a recipe** from a search box: type part of a name, or open the list. Dots show what's ready (green), short of materials (red), Edge-locked (grey) or rare and unlearned (gold).
  - **The recipe card** shows the item, its ingredients against what the character carries, the result, the roll with its modifiers, the time and any Edge, with **Craft** at the bottom. Click to choose between alternative ingredients (Psycho's Stimpak or Diluted Stimpak). The GM teaches and forgets rare recipes from the card.
  - **Mods by drag and drop** on the Weapons Workbench, Armor Workbench and Power Armor Station: pick an item, then drag a mod onto its slot, or drag it back off to take it out (each still a Repair roll). Power armor shows its Mod slots as a meter. The Robot Workbench keeps its robot and Automatron panel, restyled.
  - **The C.A.M.P.** replaces the no-station view: cooking and Break Down Junk anywhere, plus mods at −2 with a Deluxe Toolkit.
  - New bench art for all six benches and the C.A.M.P. See *12a. Workbench (Foundry Crafting)*.
- **Chems, food and drink apply their effects** (Foundry module only). Using one now puts its effect (Buffout's Strength and Vigor, Mentats' Smarts, a meal's perk) on the character who used it, for its duration, and the chat card says what's active. Before, SWADE only offered the effect on the chat card to drag onto a token. A second dose refreshes the effect instead of stacking, and nothing doubles up if SWADE or a drag already applied it.

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
