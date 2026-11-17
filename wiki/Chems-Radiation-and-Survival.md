# Chems, Radiation and Survival

## Using chems, food and drink

Use a consumable from the SWADE sheet or the Pip-Boy, and the Companion does what the item says:

- **Lasting effects** (Buffout, Mentats, Jet and so on) go onto the character as active effects for their duration, and the chat card says what's now active. A second dose of the same thing **refreshes** the effect rather than stacking it.
- **Immediate effects** (Stimpaks, RadAway, food that removes Fatigue) are applied at once, with any roll the item calls for.
- Addiction, the chem cocktail limit and the rest of the rules are in chapter 10 of [[The Book]].

## Rads

A failed radiation roll gives a **rad**. For Wild Cards, each rad takes up a Wound box, filling from the far end of the track. Rads give no penalty, and only RadAway and other treatments remove them.

- The Companion keeps the count on the character and adds a **Rads** effect that lowers their maximum Wounds, so SWADE's own Incapacitation still works.
- The standard SWADE sheet shows a **Rads** counter beside Wounds, with + and − buttons.
- On the [[The Pip-Boy Sheet|Pip-Boy]], rads show as red boxes on the Wounds row, and the rad gauge needle follows them.
- Reaching **2 rads**, and each rad after, posts a Breaking Point reminder in chat. A rad that overflows the track brings **Radiation Sickness**: the character is Incapacitated until a rad is treated.
- **Chosen of Atom:** the first rad takes up no box.
- **RadAway** removes one rad (Diluted RadAway on a Vigor roll). Brahmin Milk and Mutant Hound Chops remove one; a Refreshing Beverage removes them all.
- **Extras** take each rad as a level of Fatigue instead, marked so rest doesn't clear it.
- Worlds from 2.11 or earlier: on first load, the GM's client turns each character's marked Rad Fatigue into rads.
- Macros: `SavageFallout.addRads(actor, 1)`, `SavageFallout.removeRad(actor)`, `SavageFallout.setRads(actor, n)`, `SavageFallout.radsOf(actor)`.

## Selling salvage

With **The Stockpile** installed, Junk and trade goods sell for their full listed value (other gear sells at the usual rate), and shops use each character's caps. See chapter 12 for the rules on selling salvage.
