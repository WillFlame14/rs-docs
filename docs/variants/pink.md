---
sidebar_position: 3
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Pinkish

## Pinkish

These apply to variants with a suit that is touched by all ranks, such as Pink or Omni.

The precedence of interpreting rank clues is, from highest to lowest precedence:
1. ***Pink 1's Assumption*** (must be rank 1 when there are 1s to play and touch a new card)
1. ***Pink 8 Clue Stall*** (must be given at 8 clues, a useful rank, and touch the rightmost unclued slot)
1. ***Pink Discard*** (must be given while the receiver is *Loaded*, and touch the rightmost unclued slot and slot 1)
1. ***Pink Positional*** (must touch no new cards and target a card that can be pink)
1. Other standard interpretations, such as [*Loaded Rank Play Clue*](../learning-path/level-3#loaded-rank-play-clues), [*No-Info Double Bluff*](../learning-path/level-2#no-info-double-bluff), [*Trash Push*](../learning-path/level-3#loaded-rank-play-clues), etc.

### Good Touch Play Order
- Cards clued with a playable rank should play from **right to left**.
	- This is different from the typical playable rank order, which is left to right.

### Pink Promise
- The card that "performs" the referential action is promised to match the rank clued. This is **not necessarily** the same as the *Focus*.
- For example, this is the previously-unclued card immediately to the left to the target in the case of a *Referential Discard Clue*, and the rightmost previously-unclued card in the case of a *Lock Clue*.
- None of the other clued cards are promised to be any rank.

<figure>
    <img src={useBaseUrl('/img/pink-promise.png')} alt="Alice's slot 2 is previously clued. Bob clues 2 to Alice, touching slots 1 and 3." width="50%"/>
    <figcaption>This is a *Referential Discard Clue*, promising slot 3 to be a 2 (even though the *Focus* is slot 1).</figcaption>
</figure>

- *Pink Promise* can be broken, but should be fixed to prevent bombs.
  - When lying, the highest available rank should be clued, from [*Highest Lie Principle*](./intro#highest-lie-principle).

### Pink Promise (Reclue)
- If no new cards are clued, *Pink Promise* is on the leftmost card that was touched (as usual). This can cause a *Self-Prompt/Finesse/Bluff* if the rank is not yet playable, or indicate known trash if the rank has already been played.
	- In Dark Pink, since no pink cards can be trash, this is simply a *Pink Positional*.
- If the leftmost touched card has already been promised, the focus shifts to the next touched card to the right.
- If a player is locked, this can cause a *Direct Discard* instead of a *Self-Prompt/Finesse/Bluff*.

### Pink 1s Assumption
- This is the [same convention as in H-Group](https://hanabi.github.io/variant-specific/pink#the-1s-assumption).
- All cards touched by a 1 clue are assumed to be real 1s unless a stop clue (1, Pink or other rank) is given.
- From *Good Touch Play Order*, this means that the 1s should be played from right to left.

<figure>
    <img src={useBaseUrl('/img/pink-1s-assumption.png')} alt="Alice clues 1 to Bob, touching slots 3, 4 and 5." width="50%"/>
    <figcaption>Slot 5 is promised to be a 1. Without a fix, slots 3 and 4 are assumed to be 1s as well.</figcaption>
</figure>

**Fixing 1s**

- Cluing any rank other than 1 fixes all touched cards as unplayable pinks.
	- If no new cards are touched, *Pink Promise* applies to the card that was about to play, and slot 1 gets *PTD*.
	- If new cards are touched, it is treated as a *Referential Discard Clue* (with *Pink Promise* as normal).
- If pink is clued, the next 1 that was about to play is promised to be trash, with the others being some useful pinks.

### Pink 8 Clue Stall
- At 8 clues, Alice can clue rank (excluding playable ranks and trash) touching rightmost and slot 1 to force Bob to stall.
- If a follow-up clue is not received, Bob's **slot 1 (which is now clued)** is given permission to discard.
- This also applies to turn 1, modifying [*Starting Hand Stalls*](../learning-path/level-5#starting-hand-stalls).

### Pink Discard
- When Bob is loaded, Alice can clue rank touching the rightmost unclued slot and slot 1 as a **direct discard** on pink trash in slot 1.
	- This prevents sieving in trash pink cards while loaded.
- *Pink Promise* applies to the rightmost unclued slot.
- As mentioned in the precedence table, this overrides [*Loaded Rank Play Clues*](../learning-path/level-3#loaded-rank-play-clues) and [*Trash Push*](../learning-path/level-3#loaded-rank-play-clues).

<figure>
    <img src={useBaseUrl('/img/pink-dc.png')} alt="Alice is loaded on r3. Bob clues 5 to Alice, touching slots 1 and 3." width="50%"/>
    <figcaption>Alice is about to sieve in a trash pink by being loaded on r3, so Bob clues a *Pink Discard*.</figcaption>
</figure>

- A *Pink Discard* cannot be performed if Bob is loaded on 1s from *Pink 1s Assumption*, because any clue will look like a fix.
- In dark pinkish variants, this convention is turned off, since there are no trash pink cards.

### Pink Positional (Pink Choice Tempo Clue)
- This is the [same convention as in H-Group](https://hanabi.github.io/variant-specific/pink#the-pink-choice-tempo-clue).
- A rank clue touching no new cards **where the slot number of the rank given could be a pink card** is a *Direct Play Clue* on that slot. This helps getting pink cards that are sandwiched between other pink cards to play.
- This can be done in less-defined situations if other options are blocked.

## Pinkish-1s

In addition to the above, the following conventions apply with a pinkish-1s modification, such as Pink-1s or Omni-1s.

### Turn 1 Signal Swap
- On turn 1/2, any rank that is not 5 is treated as a rank clue of 1.
	- This is because 1 is not cluable in these variants, and this allows multiple 1s to be gotten in a single clue.
	- Note that *Good Touch Play Order* and *Pink 1s Assumption* still apply to these clues.
	- This overrides [*Starting Hand Stalls*](../learning-path/level-5#starting-hand-stalls).
- On turn 1/2, colour clues that don't target slot 1 are treated as *Referential Discard Clues*.
	- This provides some flexibility for giving discard clues.
