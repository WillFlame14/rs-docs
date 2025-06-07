---
sidebar_position: 6
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Level 7 - Edge Cases

## Special Moves

### No-Info Bluff+Prompt
- If a no-info clue is given but the receiver only has one unclued card, it calls for a *No-Info Bluff+Prompt*, with the prompt on the leftmost touched card in the no-info clue.
- If the leftmost touched card is known to be unpromptable, it moves to the right.
- If all touched cards are known to be unpromptable, it becomes the leftmost unknown card (not necessarily touched).

### 1's Order Chop Move
- This is [a similar convention to the one in H-Group](https://hanabi.github.io/level-4#the-order-chop-move-ocm), but not the same.
- Starting hand 1's should be played from left-to-right. Skipping _N_ cards means that the other player should *Chop Move* their leftmost _N_ non-*Chop Moved* cards.

### Loaded 1's Order Discard
- If the other player is loaded, all of their cards will be sieved, so it doesn't make sense to *Chop Move* any of tthem.
- Instead, skipping _N_ cards means that the other player's _N_'th unclued card from the left is known trash.

<figure>
    <img src={useBaseUrl('/img/loaded-1ocd.png')} alt="Bob is loaded with playable 1s in slots 3, 4 and 5. Alice plays her 1 in slot 5 instead of her 1 in slot 2." width="100%"/>
    <figcaption>Since Alice skipped one 1 (played slot 5 instead of slot 2), she is indicating that Bob's slot 1 is trash.</figcaption>
</figure>

## Conventions

### 8 Clue PTD
- If a rank clue is given touching rightmost and a card with 8cs *PTD*, it means to discard the card with 8cs PTD.

### PTD Revoke Exception for Loaded Rank Play Clues
- Receiving a loaded rank clue (while only loaded on *PTD*) that seems to target slot 1 instead means to reset chop to slot 1.
