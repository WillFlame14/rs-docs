---
sidebar_position: 8
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Sudoku

### Turn 1 Bomb
- Alice can bomb a card in any slot on turn 1, indicating that Bob should write *Permission to Discard* on that slot.
- Since it is turn 1, he necessarily has a duplicate of that card in his hand.

### Loaded Direct Opposite Clues
- If Alice has just been given an unknown play with at least 2 undecided stacks, she can clue the opposite type to promise that the leftmost touched card matches Bob's clue.
- For example, if Bob gave Alice a *Referential Play Clue* using blue, Alice cluing 4 promises the leftmost touched 4 is blue. This allows Bob to identify his card exactly and play it in most cases, unless it matches Alice's unknown play (i.e. Alice is about to play a non-blue 4).
- If it does match, Bob should stall by revealing or giving any other fill-in, and Alice should not play her original card.

### Sudoku Chained LDO Clues
- If Bob plays from a *LDO* clue, Alice can "chain" these clues where her promised colour travels to the left / her promised rank travels down (skipping played stacks and wrapping around).
- For example, if Alice previously promised blue, her next rank clue promises leftmost is green (unless green stack has already started, etc).