---
sidebar_position: 0
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Level 1 - Basics

This is a summary of the [*Basic Conventions*](../basics/play-clues). If you haven't read those, it's recommended to start there.

## Special Moves

### Referential Play Clues

- To get a card (the *Target*) to play, a **colour clue** is given to the unclued card immediately to its **right** (the *Focus*).
- The *Focus* of the clue is the leftmost **newly-clued** card, except slot 1 has the lowest precedence.
- The *Target* of the clue is the **previously-unclued** card to its left, wrapping around to the right side if necessary.

### Referential Discard Clues

- To get a card (the *Target*) to discard, a **rank clue** is given to the unclued card immediately to its **left** (the *Focus*).
- The *Focus* of the clue is the leftmost **newly-clued** card.
- The *Target* of the clue is the **unclued** card to its right (no wraparound).
- A discard clue that has no *Target* is a *Lock Clue*, and the receiver cannot discard any card until further information is given.

## Conventions

### Safe Actions

- A **safe action** is a known playable card or a known trash card.
- Any clue that reveals a new safe action has **no additional meaning**, even if it touches new cards.

### The Chop

- If a player has a safe action, they do not have a chop.
- When a player has no safe actions, they are given *Permission to Discard* slot 1.
- When a player receives a safe action, the card that would have been on chop moves into the hand instead, becoming **sieved**.

## Rationale

- *Referential Discard Clues* are rank instead of colour since they are less likely to be blocked when trying to discard trash.
  - For both types of clues, they will be blocked if a useful card of the same rank/colour is directly to its left.
  - However, *Playable Rank Clues* allow playable cards on the left to be played before potential trash cards on the right.
  - A potential *Playable Colour Clue* variation would only work when the particular stack is up to 4, and is thus much less useful.

- The *Lock Clue* can be thought of as a *Referential Discard Clue* that targets slot 1 (with wraparound).
  - This clue is useless, since even if this clue was not given, the default action would be to discard slot 1.
  - Thus, the clue is repurposed to have a different meaning.