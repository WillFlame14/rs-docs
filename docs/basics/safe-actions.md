---
sidebar_position: 2
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Safe Actions

- A **safe action** is a known playable card or a known trash card.
    - For level 3 players, known trash includes cards with [*Permission to Discard*](../learning-path/level-3#hard-permission-to-discard).
    - For level 5 players, known trash includes cards with [*Zero Clue Safety Promise*](../learning-path/level-5#zero-clue-safety-promise).
- Any clue that reveals a new safe action in a previously-clued card has **no additional meaning**, even if it touches new cards.

<figure>
    <img src={useBaseUrl('/img/safe-actions.png')} alt="y2 is on the play stacks. Alice clues 3 to Bob, filling in y3." width="100%"/>
    <figcaption>Alice's clue reveals a playable y3. This is not a *Referential Play Clue*.</figcaption>
</figure>

- Note that safe actions can be indicated with clues that don't touch the cards they are signalling to be playable or trash.

<figure>
    <img src={useBaseUrl('/img/safe-actions-2.png')} alt="y4 is on the play stacks. Alice clues 5 to Bob, revealing a yellow card as !5." width="100%"/>
    <figcaption>Alice's clue reveals a trash yellow card.  This is not a *Referential Discard Clue*.</figcaption>
</figure>

- However, a colour clue that reveals a new safe action in a **newly-clued** card is still referential.
    - A rank clue that reveals a new safe action in a newly-clued card is a *Playable Rank Clue*, covered below.

<figure>
    <img src={useBaseUrl('/img/safe-actions-3.png')} alt="p4 is on the play stacks. Alice clues purple to Bob, touching slot 2." width="100%"/>
    <figcaption>Alice's clue reveals p5 from [good touch](./basic-principles#good-touch-principle), but it is still a *Referential Play Clue*. Bob should play slot 1 first.</figcaption>
</figure>

## Playable Rank Clues

- A rank clue where all good touch identities of that rank are playable is a direct play on those cards.
- Cards that are playable from good touch should be played from left-to-right.

<figure>
    <img src={useBaseUrl('/img/direct-rank.png')} alt="No cards have been played. Alice clues 1 to Bob." width="100%"/>
    <figcaption>Alice's clue reveals two playable 1s. This is not a *Referential Discard Clue*.</figcaption>
</figure>
