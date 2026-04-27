---
sidebar_position: 5
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Brownish

These apply to variants with a suit that is touched by no ranks, such as Brown or Null.

### Unclued Browns
- Cards that can be brown are always unclued, as if they were null. This means that they can always be referred into and out of to get plays/discards.
	- This can be noted using a note of `[unclued]`.
- In brownish + rainbowish variants, revealing a card to be rainbow instead of brown makes it clued again. Such a clue should be interpreted as if the revealed-rainbow cards were clued for the first time.

### Permanent Chop Moves
- Cards that have been intentionally sieved in are *Chop Moved* and should be skipped over when determining a discard, until they are revealed to not be brownish.

### Trash Chop Move
- A clue revealing trash causes a [*Chop Move*](../learning-path/level-3#chop-moves) on slot 1. This overrides [*Trash Push*](../learning-path/level-3#trash-push) unless the receiver is *Loaded* or slot 1 cannot be a useful brown card.
- This is because brownish cards may block *Referential Discard Clues* from being given to sieve the card on chop.

### Brownish Save
- A rank *Reclue* touching the leftmost previously-ranked card causes a [*Chop Move*](../learning-path/level-3#chop-moves) on slot 1. This overrides [*No-Info Double Bluff*](../learning-path/level-2#the-no-info-double-bluff).
- This is because a *Trash Chop Move* is not always available, and the leftmost previously-ranked card has the rank that is least likely to be blocked.
- If no cards were previously touched with rank, a *Brownish Save* cannot be given.

<figure>
    <img src={useBaseUrl('/img/brownish-save.png')} alt="Alice's slots 2, 3, 4 and 5 are previously clued. Bob clues 5 Alice, touching slots 2 and 3." width="100%"/>
    <figcaption>This is a *Brownish Save* on slot 1, giving *PTD* to slot 2. If Bob had clued 2 or blue instead, it would be a *No-Info Double Bluff*.</figcaption>
</figure>

### Loaded 1's Order Chop Move
- Playing a 1 out of order *Chop Moves* cards as if the other player was not loaded.
- This can be used to save brownish cards that would not get a `[cm]` note otherwise.
- This overrides the [*Loaded 1's Order Discard*](../learning-path/level-8#loaded-1s-order-discard).
