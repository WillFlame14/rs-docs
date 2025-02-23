---
sidebar_position: 0
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Referential Play Clues

- The "referential" part of *Referential Sieve* indicates that cards **next to** the desired cards are clued, rather than being clued directly.

- To get a card (the *Target*) to play, a **colour clue** is given to the unclued card immediately to its **right** (the *Focus*).
    - If no new cards are clued, this is instead a [*Reclue*](../learning-path/level-2) and is covered in level 2.

<figure>
    <img src={useBaseUrl('/img/play-clue.png')} alt="Alice clues yellow to Bob, touching slot 5." width="50%"/>
    <figcaption>This clue means to play slot 4 (focuses slot 5).</figcaption>
</figure>

When multiple cards are clued,
- The *Focus* of the clue is the leftmost **newly-clued** card, except slot 1 has the lowest precedence.
- The *Target* of the clue is the **previously-unclued** card to its left, wrapping around to the right side if necessary.

<figure>
    <img src={useBaseUrl('/img/play-clue-2.png')} alt="Alice clues yellow to Bob, touching slot 1. Slots 2 and 5 are previously clued." width="50%"/>
    <figcaption>This clue means to play slot 4 (focuses slot 1).</figcaption>
</figure>

- Note that play clues can target newly-clued cards as well.

<figure>
    <img src={useBaseUrl('/img/play-clue-3.png')} alt="Alice clues yellow to Bob, touching slots 1, 2 and 3. Slots 2 and 5 are previously clued." width="50%"/>
    <figcaption>This clue means to play slot 1 (focuses slot 3).</figcaption>
</figure>
