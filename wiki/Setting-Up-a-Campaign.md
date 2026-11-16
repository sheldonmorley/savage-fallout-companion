# Setting Up a Campaign

A checklist for GMs. Everything is optional: use the parts your game needs.

## Characters

- New characters start with the Fallout core skills (set up automatically the first time the module loads).
- Character and NPC sheets get a Vault-Tec blue-and-yellow theme. Turn it off with **Fallout sheet theme** in the settings.
- Players can switch to the [[The Pip-Boy Sheet|Pip-Boy sheet]] in their character's sheet settings.

## Workbenches

Drag stations from **Fallout Workbench Stations** onto your scenes: Weapons Workbench, Armor Workbench, Power Armor Station, Chemistry Station, Cooking Station, Robot Workbench. Players double-click them to craft. See [[Workbench and Crafting]].

Hand out **rare recipes** from **Fallout Crafting Materials > Rare Recipes** as loot or rewards, or teach them from the Workbench.

## Scavenging

Drop **Scavenge Nodes** on your maps, or add tile, region or journal-button searches. Run **Restock Scavenging (This Scene)** when the wasteland should refill. See [[Scavenging]].

## The world map

The Companion ships no world map, so each campaign uses its own.

1. Create a scene with your world map as its background image.
2. In the module settings, pick that scene under **Pip-Boy world map**. (If a new scene isn't in the list yet, reload once.)
3. Place **map pins** on that scene for the locations. The pin icon list includes 62 Pip-Boy location icons, named *Pip-Boy: Vault*, *Pip-Boy: Settlement* and so on, plus *Quest Destination*, *Signal Source* and location pins.
4. Link each pin to a journal entry, and reveal it by permission:
   - **None**: the player doesn't see the location.
   - **Limited**: the player sees its outline (undiscovered).
   - **Observer**: the player sees the filled icon and can open the entry.

The Pip-Boy swaps between each location's found and undiscovered icon by itself. Pins with no journal entry show to everyone. A character's token on the map scene shows as *you are here*.

## Radio

- The Companion's **Fallout Radio** is always available; it plays from the module's own files.
- Add your own stations: put playlists in a world playlist folder named **Radio** (or the name set in **Pip-Boy radio folder**), and give players **Observer** permission on them.
- Players hear their radio on their own computer only. As GM, tick **Play for the whole table** on the Pip-Boy to play a station for everyone.

## Quests and notes

- Make journal folders named **Quests** and **Notes** (or the names in the settings).
- Share an entry with a player (Observer) and it appears on their Pip-Boy.
- Move finished quests into a subfolder named **Completed** to show them as Done.

## Landing page

The **Fallout Scenes** compendium includes two landing-page scenes you can use as a world's opening screen. A button on a landing page can open a player's Pip-Boy with `SavageFallout.openPipBoy()`.
