# The Pip-Boy Sheet

An alternate character sheet that shows your character on a working Pip-Boy. It reads the same character as the SWADE sheet, live, so the two are always in step. Use it for what you check and do most at the table; the SWADE sheet is still there for building and editing.

## Turning it on

- Open a character, open its sheet settings (**Sheet**, or **Configure Sheet** in the title bar's menu), and choose **Pip-Boy**. Each player can choose it for their own character. It works for NPCs too.
- Or run `SavageFallout.openPipBoy()` from a macro. It opens your assigned character (or the selected token). `SavageFallout.openPipBoy({ tab: "inv" })` opens a tab directly; tabs are `stat`, `inv` and `data`.

## The controls

- **Three knobs** under the screen switch between **STATS**, **ITEMS** and **DATA**. The one in use lights up.
- **The dial** on the left steps through the sub-tabs. Click it, or scroll over it. The labels along the bottom of the screen work too.
- **The rad gauge** at the top left follows your Rad Fatigue.
- The window can be resized and everything scales with it.
- Clicks make Pip-Boy sounds at your interface volume. Turn them off in the module settings (each player chooses for themselves).

With the **Pip-Boy frame folder** setting cleared, the sheet draws a plain green screen with tabs along the top instead of the frame.

## STATS

- **Status**: Wounds, Fatigue and Rad Fatigue as rows of boxes. Click a box to set the track to that level; click the last filled box to clear it. Also conditions (Shaken and so on), active effects with the time left, and Pace, Parry, Toughness and Bennies.
- **Rad Fatigue** marks which Fatigue levels came from radiation, as the Radiation rules ask. Marked levels show hatched on the Fatigue row. Marking Rad Fatigue adds the Fatigue too. RadAway removes a marked level; anything else that lowers Fatigue takes the mark down with it.
- **Attributes** and **Skills**: pick one and click **Roll**.
- **Edges**: Edges, Hindrances and ancestry abilities, with their full text.

## ITEMS

- **Weapons, Apparel, Aid, Misc, Ammo**, with weight carried against your load limit, Armor and caps along the top. A filled square marks equipped gear. Each item shows its own art, tinted green.
- **Attack** posts the weapon's chat card, with its attack and damage buttons.
- **Equip / Unequip** moves weapons to the main hand, shields to the off hand and armor onto the body. Use the SWADE sheet for two-handed or off-hand weapons.
- **Use** on a chem, food or drink spends one dose and applies it, exactly as using it from the SWADE sheet does.
- **Learn** on a found recipe (under Misc) teaches it to you. See [[Workbench and Crafting]].
- **Open** opens any item's own sheet.

## DATA

- **Quests**: the journal entries in a folder named *Quests*. You see only the entries the GM has shared with you. Entries in a *Completed* subfolder show as Done, at the bottom.
- **Notes**: the same, from a folder named *Notes* (holotapes, letters, terminal entries).
- **Map**:
  - **WORLD** shows the scene the GM picked as the world map, tinted green. **LOCAL** shows the scene you're on.
  - Drag to pan; scroll or use **+** and **−** to zoom. Your token shows as *you are here*.
  - Markers are the scene's map pins. A pin's journal entry at **Limited** shows the location's outline (undiscovered); at **Observer** it shows the filled icon, and **Open** reads the entry. Pins with no journal entry show to everyone.
- **Radio**:
  - Stations are the Companion's **Fallout Radio** plus any playlists in a world folder named *Radio*.
  - **Tune in** plays a station in shuffled order **on your computer only**. It uses your music volume and the Pip-Boy's own volume slider, and keeps playing with the Pip-Boy closed. **Next track** skips; **Turn off** stops.
  - Players can't play a station for the table. The GM gets a **Play for the whole table** box that plays it as an ordinary playlist.

GMs: see [[Setting Up a Campaign]] for the world map, map pins, radio and quest folders.
