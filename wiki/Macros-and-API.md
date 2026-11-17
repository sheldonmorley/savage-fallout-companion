# Macros and API

## Macros

In the **Fallout Macros** compendium:

| Macro | What it does |
|---|---|
| **Open Workbench** | Opens the C.A.M.P. for the selected token or your character. |
| **Break Down Junk** | Breaks down Junk and unwanted gear into Resources. |
| **Scavenge Here** | A one-off search with no node, using the preset named in the macro (edit it to taste). |
| **Restock Scavenging (This Scene)** | Restocks every scavenging node, tile and region on the current scene. |

## API

Everything is on `SavageFallout` (also `game.modules.get("fallout-companion").api`). Use these in macros, Monk's Active Tiles, Region behaviors or landing-page buttons.

### Pip-Boy

```js
SavageFallout.openPipBoy();                       // your character, or the selected token
SavageFallout.openPipBoy({ tab: "data" });        // "stat", "inv" or "data"
SavageFallout.openPipBoy({ actor: someActor });
```

### Rads

```js
SavageFallout.radsOf(actor);          // how many rads
SavageFallout.addRads(actor, 1);      // add rads (Wild Cards: Wound boxes; Extras: marked Fatigue)
SavageFallout.removeRad(actor);       // remove one, as RadAway does
SavageFallout.setRads(actor, 0);      // set the count
```

### Workbench

```js
SavageFallout.openWorkbench();                                // the C.A.M.P.
SavageFallout.openWorkbench({ station: "chemistry" });        // weapons, armor, powerArmor, chemistry, cooking, robot
SavageFallout.openWorkbench({ actor: someActor, station: "weapons" });
SavageFallout.breakDownJunk();                                // the Break Down Junk dialog
```

### Scavenging

```js
SavageFallout.scavenge({ preset: "footlocker", node: tile });
SavageFallout.scavenge({ preset: "ruined-house", node: region, actor, degree: "untouched", tier: "rich" });
SavageFallout.resetScavenge(page, "farmhouse");   // restock one journal button (or pass a tile, region or token)
SavageFallout.resetScavengeScene();               // restock the current scene
SavageFallout.presets;                            // the stock and add-on presets
```

`scavenge` options: `actor`, `node` (a tile, region, token, journal page or UUID, where the search history is kept), `key`, `preset`, and any of `name`, `scale`, `degree`, `tier`, `skill`, `readAs`, `table`, `lock`, `salvage`, `maxCards`. See [[Scavenging]].

### Mods (outside the Workbench)

```js
SavageFallout.installModDialog(actor);   // pick a mod and an item, roll, install
SavageFallout.removeModDialog(actor);    // pick an item and one of its mods, roll, remove it intact
```
