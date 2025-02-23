---
sidebar_position: 2
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Level 3 - Loaded Situations

## Special Moves

### Loaded Clues

- A player is *Loaded* if they have a safe action.
- If a player has more than one safe action, note that some of the cards they draw will never be on chop.
	- Those cards will be "automatically sieved" as the player performs their safe actions.
- Thus, cluing *Loaded* players is low-value, since they'll end up with more than one safe action and trash cards might be sieved into their hand.

### Loaded Rank Play Clues

- A *Loaded* player will never discard their chop, so it doesn't make sense to give them a *Referential Discard Clue*.
- A rank clue while loaded is instead a signal to play the card to the right of the newly-clued cards.
  - The rank must not be known trash, otherwise it becomes a *Trash Push* (see below).

When multiple cards are clued, 
- The *Focus* of the clue is the rightmost **newly-clued** card, but the rightmost previously-unclued card has lowest precedence.
- The *Target* of the clue is the **previously-unclued** card to its right, wrapping around if necessary.

This works in essentially the same way as a *Referential Play Clue*, but toward the right instead of the left.

In the following example, Bob was previously given a *Referential Discard Clue* targeting slot 4.
<figure>
    <img src={useBaseUrl('/img/loaded-rank-play.png')} alt="Bob is loaded with a safe discard. Alice clues 3 to Bob, touching slot 1." width="100%"/>
    <figcaption>Alice is calling for Bob's slot 2 to play.</figcaption>
</figure>

### Loaded Colour Clues

- Colour clues have the same meaning while loaded (i.e. [*Referential Play Clues*](../basics/play-clues)).
- Previously-targeted cards are skipped over when determining the *Target*.

### Trash Push
- A clue that touches only known trash is a *Trash Push*. If the receiver is *Loaded*, this has higher precedence than a *Loaded Rank Play Clue*.
- This is interpreted as if a colour clue was given touching the same cards, as a [*Referential Play Clue*](../basics/play-clues).
    - If the targeted card is clearly unplayable, the target shifts left (with wraparound) until reaching a potentially playable card.

<figure>
    <img src={useBaseUrl('/img/trash-push.png')} alt="All 1s have been played. Alice clues 1 to Bob, touching slots 1, 2, 3, 5." width="100%"/>
    <figcaption>Alice is calling for Bob's slot 4 to play.</figcaption>
</figure>

## Conventions

### Hard Permission to Discard

- When a card receives *Permission to Discard*, it is considered to be known trash. Discarding a card with *PTD* is thus considered to be a safe action, and a player that has a card with *PTD* is *Loaded*.
- This means that they can receive *Loaded Rank Play Clues*, and they **do not have a chop** until the card with *PTD* is discarded.
- This means that both players need to keep track of the everyone's safe actions, in order to determine which cards have *PTD* and when someone becomes *Loaded*.
- It helps to keep track of the card that has *PTD* by writing a note of `[kt]` on it.

### Revoking PTD

- If necessary, *PTD* can be revoked by cluing the card directly. This can occur due to double discard situations, for example.
- Such a clue should be interpreted as if the player did not previously have *PTD*.

### Chop Moves

- If a card is intentionally sieved in and doesn't receive *PTD*, the card must be important.
- This can be noted using a note of `[cm]`, which stands for *Chop Move*.
- *Chop Moved* cards are not special: the note is purely for personal information and such cards can still be targeted by *Referential Discard Clues*.
    - This is different from H-Group, where cards that have been *Chop Moved* are no longer eligible to be discarded.
