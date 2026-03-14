---
sidebar_position: 3
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# The Chop

## The Chop

- The "sieve" part of *Referential Sieve* indicates that slot 1 acts like a sieve for cards entering the hand.
- When a player has no safe actions, they are given *Permission to Discard* slot 1.
    - This is called the **chop**, since it's like the card is on the "chopping block".
- If a player has a safe action, they do not have a chop.

<figure>
    <img src={useBaseUrl('/img/chop.png')} alt="Alice has r2 in slot 1, and Bob has y1 in slot 1." width="50%"/>
    <figcaption>Alice's chop is r2, and Bob's chop is y1.</figcaption>
</figure>

- Note that when a player receives a safe action, the card that would have been on chop instead moves into the hand.

<figure>
    <img src={useBaseUrl('/img/play-clue.png')} alt="Alice clues yellow to Bob, touching slot 5." width="50%"/>
    <figcaption>After Bob plays slot 4 (from the *Referential Play Clue*), he will get a new chop.</figcaption>
</figure>

- That card is now **sieved**. As cards can only move toward the right of one's hand, it will never be on chop again.
- Sieving trash cards into the hand is very bad, because additional clues will be needed to make them discard!

## Managing the chop

- Your partner should always either have a safe action or a safe chop (i.e. not playable or critical).
- If your partner's chop is important, a clue should be given to save it!

<figure>
    <img src={useBaseUrl('/img/managing-chop.png')} alt="Alice's hand is g5, p2, b3, g2, b3." width="50%"/>
    <figcaption>To prevent Alice from discarding g5, Bob can clue 2 to Alice (as a *Referential Discard Clue*).</figcaption>
</figure>

- Giving any safe action will move the card on slot 1 off chop.
    - This includes [*Referential Play Clues*](./play-clues) and fill-in clues that reveal a safe action.

<figure>
    <img src={useBaseUrl('/img/managing-chop-2.png')} alt="y1 is played. Alice's hand is p3, y5, g2, y2, b3." width="100%"/>
    <figcaption>To prevent p3 from being discarded, Bob can clue blue to Alice (as a *Referential Play Clue*).</figcaption>
</figure>
