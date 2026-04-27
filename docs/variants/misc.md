---
sidebar_position: 8
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Other Variants

### Non-Orange Assumption
- In variants with an orange suit, rank-clued cards whose good-touch suits are all playable are assumed to be not orange (i.e. they can be dragged to the stacks).
	- Note that the orange suit must also be at or above the playable rank.
- This follows *Good Touch Play Order* (left-to-right).
- If the card is orange, an orange clue can be used to fix and is not additionally referential.

### Orange Play Meaning
- A *Referential Play Clue* targeting an Orange card means to drag it to the play stacks (discard it).
	- This is because if we wanted it to be dragged to the discard pile (play it), we would do nothing and let it receive *PTD*.

### Ambigous Prism Tempo Clue
- This is the [same convention as in H-Group](https://hanabi.github.io/variant-specific/prism/#the-ambiguous-prism-tempo-clue).
- Colour is a *Tempo Clue* on the right card, rank is a *Tempo Clue* on the left card.

### 1's Play Promise
- A 1 clue on turn 1 always indicates playable 1s (left to right in all variants except *Pink*-ish).
- This applies to *Orange*, *Reversed* and *Up and Down* variants.

### Reversed 1's Save
- A 1 clue after turn 1 in *Reversed* always has to be respected as touching the reversed 1.

### Up or Down Loaded Direct Colour Clues
- In *Up or Down*, a colour clue while the ***giver*** is loaded means that the leftmost touched card can start the stack. If the stack for that colour has already started, the clue is treated as a *Referential Play Clue*.
	- This is different from the [*Loaded Colour Clues*](../learning-path/level-3#loaded-colour-clues) convention, which requires that the ***receiver*** is loaded.
- If a *Loaded Direct Colour Clue* is given while the giver is loaded on the same colour, the receiver should respond with the clue matching the card.
	- colour for START cards (giver should play START next)
	- rank for 1/5 cards (giver should respond with colour if receiver has START, otherwise giver should play their own card next)
- If giver plays, the receiver receives *PTD* on the leftmost unclued slot. Thus, giver can follow up with a rank clue after receiver responds if slot 2 is not safe, which is **not** loaded.
