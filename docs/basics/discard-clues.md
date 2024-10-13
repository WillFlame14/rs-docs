---
sidebar_position: 1
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Referential Discard Clues

- The "referential" part of *Referential Sieve* indicates that cards **next to** the desired cards are clued, rather than being clued directly.
- To get a card (the *Target*) to discard, a **rank clue** is given to the unclued card immediately to its **left** (the *Focus*).
    - If no new cards are clued, this is instead a *Reclue* and is covered in level 2.

<figure>
    <img src={useBaseUrl('/img/discard-clue.png')} alt="Alice clues 4 to Bob, touching slot 3." width="50%"/>
    <figcaption>This clue means to discard slot 4 (focuses slot 3).</figcaption>
</figure>

When multiple cards are clued, 
- The *Focus* of the clue is the leftmost **newly-clued** card.
- The *Target* of the clue is the **unclued** card to its right.

<figure>
    <img src={useBaseUrl('/img/discard-clue-2.png')} alt="Alice clues 5 to Bob, touching slots 1 and 5. Slots 2 and 3 are previously clued." width="50%"/>
    <figcaption>This clue means to discard slot 4 (focuses slot 1).</figcaption>
</figure>

## Lock Clues

- A discard clue that has no *Target* is a *Lock Clue*.
- A player that is *Locked* is not allowed to discard any card until further information is given.
- Special rules around *Locked* players are explained in [level 4](../learning-path/level-4).

<figure>
    <img src={useBaseUrl('/img/lock-clue.png')} alt="Alice clues 5 to Bob, touching slots 4 and 5. Slot 5 is previously clued." width="50%"/>
    <figcaption>This clue locks Bob (focuses slot 4).</figcaption>
</figure>
