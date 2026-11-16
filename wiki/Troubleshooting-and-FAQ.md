# Troubleshooting and FAQ

**An update fails with "EACCES" or "permission denied".**
An old release made some of the module's folders read-only. Uninstall the module and install it again from the manifest, or make the folder writable. On a Mac:
```
chmod -R u+w ~/Library/Application\ Support/FoundryVTT/Data/modules/fallout-companion
```
Your world's data isn't affected either way.

**Foundry still offers the old version after a release.**
GitHub can take a few minutes to show the new `module.json`. Wait, then check for updates again.

**A scavenging search doesn't do anything.**
A GM has to be logged in: the GM's client draws the cards and hands out the loot.

**My radio station doesn't show on the Pip-Boy.**
The playlist must be in the folder named in **Pip-Boy radio folder** (default *Radio*), and players need **Observer** permission on it.

**A location doesn't show on the Pip-Boy map.**
Its pin's journal entry needs at least **Limited** permission for that player (Observer to show it as found). Pins must sit inside the scene's map area. If the world map scene isn't in the settings list, reload once.

**Can players play music for the whole table?**
No. A player's Pip-Boy radio plays only on their own computer; only the GM can play a station for everyone.

**I used a found recipe and nothing happened.**
If the character already knows the recipe, or lacks an Edge it needs, it isn't learned and isn't used up. A notification says which.

**Does the module change the rules?**
No. Everything it automates is in [[The Book]]; the book is the rules.

**Which other modules do I need?**
Only the SWADE system and the SWADE Core Rules module. The Stockpile and Monk's Active Tiles are optional extras.

Found a bug? Open an issue: https://github.com/sheldonmorley/savage-fallout-companion/issues
