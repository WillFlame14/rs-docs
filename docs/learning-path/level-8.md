---
sidebar_position: 7
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Level 8 - Advanced Moves

## Special Moves

### Self-Connecting Priority
- If a player has two playable cards, one of which connects to their own hand and the other doesn't connect to anything, playing the connecting card is often better.
- Thus, playing the non-connecting card is a *Priority Prompt* on the rightmost card that could reasonably be the connecting card, or a *Priority Finesse/Bluff* on the leftmost unclued card.

In the following example, Alice's y4 is clued only with yellow.

<figure>
    <img src={useBaseUrl('/img/self-connecting-prio.png')} alt="Bob has known b3, b4 and y3, with the blue and yellow stacks both at 2. Alice has a y5 on chop." width="100%"/>
    <figcaption>Bob can play y3 as a *Self-Connecting Priority Prompt*, thus not needing to save Alice's y5 on chop.</figcaption>
</figure>

## Conventions

### Quasi-Locked
- If Alice is given a *Referential Discard Clue* and could be discarding a useful card while Bob has known trash (including *PTD*), she can stall for 1 turn by giving a *Fill-In Clue* to Bob or a direct colour clue (focusing leftmost). This is **not** additionally referential.
- If Bob plays, it is treated as *Unlock Promise* on Alice, targeting the card called to discard. Otherwise, Bob should discard.
- This prevents the situation where Alice is forced to discard a 1-away card that connects through an unknown card in Bob's hand.
- In rainbowish variants, [*Colour Truth*](../variants/rainbow#quasi-locked-colour-truth) applies to this convention.

In the following example, Alice has previously told Bob's slot 2 to discard. Alice also has *PTD* in slot 1.

<figure>
    <img src={useBaseUrl('/img/quasi-locked.png')} alt="Bob clues green to Alice, touching slots 4 and 5." width="100%"/>
    <figcaption>Bob is promising g2 in Alice's slot 4. Alice should play slot 4, causing Bob to *Unlock Promise* g3 in slot 2.</figcaption>
</figure>
