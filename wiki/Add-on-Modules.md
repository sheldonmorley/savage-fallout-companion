# Add-on Modules

Other modules can extend the Companion without changing it. The Companion only reads from add-ons that are installed and switched on; with none, nothing changes.

## Adding recipes

In your module's `module.json`, point a flag at a recipes file in the same format as the Companion's `scripts/recipes.json`:

```json
"flags": {
  "fallout-companion": { "recipes": "modules/your-module/recipes.json" }
}
```

The Workbench merges those recipes in. Each recipe names its bench (`station`), skill, Complexity, any Edges, its ingredients and its product (an item UUID). Mark a recipe `"rare": true` to make it rare; give a found-recipe item the flag `flags["fallout-companion"].teaches = "<recipe id>"` and using it teaches that recipe.

## Adding scavenging locations

Add-ons can register their own scavenging presets (new locations, or regional loot using a roll table instead of cards). They then work everywhere a stock preset does: nodes, tiles, regions and `@Scavenge` buttons.

## Automatron parts

Robot parts carry their data in an item flag (`flags["fallout-companion"].part`, or under the add-on's own namespace). Installing a part on a robot at the Robot Workbench applies it: attribute and Pace changes, Armor, Toughness and Parry, skill steps, extra Mod Slots, granted items and abilities. Slots are one each for torso, legs, head and armor, two arms, and one attachment per arm.

Questions about the formats: open an issue on GitHub.
