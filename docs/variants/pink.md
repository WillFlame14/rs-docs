---
sidebar_position: 3
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Pinkish

These apply to variants with a suit that is touched by all ranks, such as Pink or Omni.

The precedence of interpreting rank clues is, from highest to lowest precedence:
- *Pink 1's Assumption*
- *Pink 8 Clue Stall*
- *Pink Discard*
- *Pink Positional*
- *Pink Promise*
- *Loaded Rank Play Clue*

### Good Touch Play Order
- Cards clued with a playable rank should play from **right to left**.

### Pink 1s Assumption
- This is the [same convention as in H-Group](https://hanabi.github.io/variant-specific/pink#the-1s-assumption).
- All cards touched by a 1 clue are assumed to be real 1s unless a stop clue (1, Pink or other rank) is given.

**Fixing 1s**

- Cluing any rank other than 1 fixes all touched cards as unplayable pinks.
	- If no new cards are touched, *Pink Promise* applies to the card that was about to play, and slot 1 gets *PTD*.
	- If new cards are touched, it is treated as a *Referential Discard Clue* (with *Pink Promise* as normal).
- If pink is clued, the next 1 that was about to play is promised to be trash, with the others being some useful pinks.

### Pink 8 Clue Stall
- At 8 clues, Alice can clue a rank clue touching rightmost and slot 1 to force Bob to stall. If a follow-up clue is not received, Bob's slot 1 is given permission to discard.
- This also applies to turn 1 (modifying *Starting Hand Stalls*).

### Pink Discard
- When Bob is loaded, Alice can clue rank touching rightmost and slot 1 as a direct discard on pink trash in slot 1.
- This prevents sieving in trash pink cards while loaded.

### Pink Positional (Pink Choice Tempo Clue)
- This is the [same convention as in H-Group](https://hanabi.github.io/variant-specific/pink#the-pink-choice-tempo-clue).
- A rank clue touching no new cards, where the slot number of the rank given could be a pink card, is a *Direct Play Clue* on that slot. This helps getting pink cards that are sandwiched between other pink cards to play.
- This can be done in less-defined situations if other options are blocked.

### Pink Promise
- The card that performs the referential action in a newly touched card is promised to match the rank clued.
- For example, this is the previously unclued card immediately to the left to the discarded card in the case of a *Referential Discard Clue*, and the rightmost card in the case of a lock. None of the other clued cards are promised to be any rank.
- *Pink Promise* can be broken, but should be fixed to prevent bombs.

### Pink Promise (Reclue)
- If no new cards are clued, *Pink Promise* is on the leftmost card that was touched (as usual). This can cause a *Self-Prompt/Finesse/Bluff* if the rank is not yet playable, or indicate *Trash* if the rank has already been played†.
	- In Dark Pink, since no pink cards can be trash, this is simply a *Pink Positional*.
- If the leftmost touched card has already been promised, the focus shifts one to the right.
- If a player is locked, this can cause a *Direct Discard* instead of a *Self-Prompt/Finesse/Bluff*.
