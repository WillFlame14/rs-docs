---
sidebar_position: 2
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Level 3 - Loaded Situations

## Special Moves

### Loaded Clues

- A player is *Loaded* if they have a safe action.
- If a player has more than one safe action, note that some of the cards they draw will never be on chop.
	- They will be "automatically sieved" as the player performs their safe actions.
- Thus, giving clues to *Loaded* players is low-value, since trash cards might end up being sieved into the hand.

### Loaded Rank Play Clues

- A *Loaded* player will never discard their chop, so it doesn't make sense to give them a *Referential Discard Clue*.
- A rank clue while loaded is instead a signal to play the card to the right of the newly-clued cards.

When multiple cards are clued, 
- The *Focus* of the clue is the rightmost **newly-clued** card, but the rightmost previously-unclued card has lowest precedence.
- The *Target* of the clue is the **previously-unclued** card to its right, wrapping around if necessary.

This works in essentially the same way as a *Referential Play Clue*, but toward the right instead of the left.

In the following example, Bob has previously been given a *Referential Discard Clue* targeting slot 4.
<figure>
    <img src={useBaseUrl('/img/loaded-rank-play.png')} alt="Bob is loaded with a safe discard. Alice clues 3 to Bob, touching slot 1." width="100%"/>
    <figcaption>Alice is calling for Bob's slot 2 to play.</figcaption>
</figure>

### Loaded Colour Clues

- Colour clues have the same meaning while loaded (i.e. *Referential Play Clues*).
- Previously-targeted cards are skipped over when determining the *Target*.

### Trash Push
- A clue that touches only known trash is a *Trash Push*.
- This should be interpreted as if a colour clue was given as a *Referential Play Clue*.
    - However, slot 1 no longer has the lowest precedence as the *Focus*.

<figure>
    <img src={useBaseUrl('/img/trash-push.png')} alt="All 1s have been played. Alice clues 1 to Bob, touching slots 1, 2, 3, 5." width="100%"/>
    <figcaption>Alice is calling for Bob's slot 4 to play.</figcaption>
</figure>

## Conventions

### Hard Permission to Discard

- When a card receives *Permission to Discard*, it is considered to be known trash. Discarding a card with *PTD* is thus considered to be a safe action, and that player is *Loaded*.
- This means that they can receive *Loaded Rank Play Clues*, and they **do not have a chop** until the old *PTD* is discarded.
- This means that both players need to keep track of the everyone's safe actions, in order to determine which cards have *PTD* and when someone becomes *Loaded*.
- It helps to keep track of the card that has *PTD* by writing a note of `[kt]` on it.

### Revoking PTD

- If necessary, *PTD* can be revoked by cluing the card directly. This can occur due to double discard situations, for example.
- Such a clue should be interpreted as if the player did not previously have *PTD*.

### Chop Move Notes

- If a card is intentionally sieved in and doesn't receive *PTD*, the card must be important.
- This can be noted using a note of `[cm]`, which stands for *Chop Move*.
- *Chop Moved* cards are not special: the note is purely for personal information and such cards can still be targeted by *Referential Discard Clues*.
    - This is different from H-Group, where cards that have been *Chop Moved* are no longer eligible to be discarded.
