# Scavenging

Every search in the Scavenging rules can run itself. A player clicks something on the map or in a journal and makes the Notice (or Survival) roll in SWADE's usual roll window. The GM's client then draws the loot cards, reads them on the Scavenging Loot tables, adds the items, caps and Junk to that character, and posts the result in chat.

- No other modules are needed, and players never need permission on tiles or journals.
- **A GM must be logged in** for searches to resolve.

## What a search does

- **Modifiers**: the location's Degree, a cumulative −2 for each earlier search there, and +2 for the Scavenger Edge (Investigator's +2 doesn't stack with it).
- **Success**: 2d6 caps' worth of salvage, as Junk. Scavenger doubles it; Scrounger adds an extra supply find.
- **Each raise**: one loot card, up to the location's maximum (Tiny and Small 1, Average 2, Large 3). Scavenger adds one more, even past the maximum. Firearms come with 2d6 rounds.
- **Jokers**: a roll on the Jackpot table, and a reminder that every hero gets a Benny.
- **Critical Failure**: a Scavenging Complication, and the location is picked clean.
- **Locks**: locked containers get a **Pick the lock** button in the chat card.
- Results that need a GM's decision (a note or holotape, a key, a rare recipe, a Bobblehead) are listed at the bottom of the card to hand out.

## Three ways to place a search

### Scavenge Node tokens

Drag a node from the **Fallout Scavenge Nodes** compendium onto the map; there's one for each stock location. A player double-clicks it to search with their character. When the GM double-clicks it, a settings window opens: change the preset, Scale, Degree, Tier, skill, which suits the cards are read as, a roll table to use instead of cards, or a lock; search as any character; or restock it.

### Tiles and Regions

Draw a tile or region and run a script. With Monk's Active Tiles (run as the triggering player):

```js
SavageFallout.scavenge({ preset: "footlocker", node: tile });
```

For a Region's Execute Script behavior (Token Enters), only the player who moved should search:

```js
if (event.user !== game.user) return;
SavageFallout.scavenge({ preset: "ruined-house", node: region, actor: event.data.token?.actor });
```

Add any setting beside the preset: `degree: "untouched"`, `tier: "rich"`, `skill: "Survival"`, `readAs: ["hearts"]`, `table: "<roll table UUID>"`, `lock: { skill: "Thievery", mod: -2, tool: "Bobby Pin" }`, `name: "Mayor's Desk"`.

### Journal buttons

Type this in any journal page and it becomes a button:

```
@Scavenge[ruined-house id=farmhouse]{Search the farmhouse}
```

The first word is the preset; add settings after it (`degree=untouched tier=rich readAs=hearts,diamonds lock=Thievery:-2 name="Mayor's Desk"`). Give each button on a page its own `id`. A searched button shows a dashed border; a picked-clean one is struck through.

## Stock locations

| Preset | Location | Scale | Degree | Tier | Notes |
|---|---|---|---|---|---|
| `footlocker` | Footlocker | Tiny | Lightly Searched | Standard | |
| `car-trunk` | Car Trunk | Tiny | Picked Over | Standard | |
| `ammo-box` | Ammo Box | Tiny | Lightly Searched | Standard | cards read as ♣ |
| `first-aid-box` | First Aid Box | Tiny | Lightly Searched | Standard | cards read as ♥ |
| `vending-machine` | Vending Machine | Tiny | Picked Over | Poor | cards read as ♥ |
| `desk` | Desk or Filing Cabinet | Tiny | Lightly Searched | Poor | cards read as ♦ |
| `wall-safe` | Wall Safe | Tiny | Untouched | Rich | ♦; locked (Thievery −2) |
| `body` | Body | Tiny | Lightly Searched | Standard | looting the fallen; searched once |
| `shack` | Shack or Single Room | Small | Picked Over | Poor | |
| `vertibird` | Wrecked Vertibird | Small | Lightly Searched | Rich | Survival |
| `raider-stash` | Raider Stash | Small | Untouched | Rich | |
| `police-armory` | Police Armory | Small | Untouched | Rich | ♣ or ♠; terminal (Hacking −2) |
| `ruined-house` | Ruined House | Average | Picked Over | Standard | |
| `gas-station` | Gas Station | Average | Picked Over | Standard | |
| `shop` | Shop or Store | Average | Lightly Searched | Standard | |
| `clinic` | Clinic | Average | Lightly Searched | Standard | ♥ or ♦ |
| `crash-site` | Crash Site or Overpass | Average | Lightly Searched | Standard | Survival |
| `vault-room` | Vault Room | Average | Untouched | Legendary | |
| `factory-floor` | Factory Floor | Large | Picked Over | Rich | |
| `military-depot` | Military Depot | Large | Untouched | Legendary | terminal (Hacking −4) |

[[Add-on Modules]] can add their own presets.

## Roll tables instead of cards

A node with a roll table rolls it once for each card it would draw. Results that link to an item give that item; text results give the item with that name, with a quantity in brackets if there is one (`Cram (1d3)`). Anything else is listed for the GM.

## Restocking

- **Restock Scavenging (This Scene)** macro: restocks every node, tile and region on the current scene.
- A single token: from its settings window.
- Journal buttons: `SavageFallout.resetScavenge(page, "id")`.

The **Whisper scavenging results** setting shows each search only to the GM and the player who made it.
