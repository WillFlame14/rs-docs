---
sidebar_position: 3
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Level 4 - Locked Hands

- A player is *Locked* after they receive a *Lock Clue*, and cannot discard any cards until further information is given.
- While they are *Locked*, the types of clues they can give are restricted so that they can be unlocked efficiently.
- When pace is greater than 2, it is better for the unlocked player to discard instead of playing a card that doesn't connect to one of the locked player's cards.
	- Thus, it is important that the unlocked player has full information about their playable cards.

## Conventions

### Colour Clues While Locked

- Any colour clue not touching slot 1 is a *Colour Stall*.
- If a colour clue touches slot 1, it means that slot 1 is playable.

### Rank Clues While Locked

- *Playable Rank Clues* and *Referential Discard Clues* are the same as while unlocked.
- *Loaded Rank Play Clues* are interpreted as *Referential Discard Clues*.
- *Reclues* and *Lock Clues* are interpreted as a stall.

### Locked Hand PTD

- Except for *Playable Rank Clues*, every clue given by the locked player promises a safe discard, known as *Locked Hand PTD*.
	- For *Referential Discard Clues*, this is simply the card called to discard.
	- For *Colour Stalls* and *Lock Clues*, this is slot 1.
	- For colour clues touching slot 1, this is the leftmost unclued card.

- If every card in the unlocked player's hand becomes clued, they do not receive *LH PTD*.

### Unlock Promise

- If the unlocked player chooses to play a **fully-known** card even when they have *Locked Hand PTD*, this promises that the locked player can become unlocked.
- The locked player should first try to connect in the same suit.
- If no cards could connect, then they should try the card most likely to be playable, biasing rightmost.
- If the unlocked player could be trying to connect through multiple cards in their own hand (e.g. r3, r4 to connect to a potential r5), then the locked player should continue to stall.
- If the unlocked player plays a card that is not commonly known, this does not promise an unlock.

### Unlock Promise Shifting

- If the unlocked player chooses to delay before playing a connecting card, this causes the unlock target to shift.
- A **delay** is any action that is not forced.
	- For example, choosing to discard *LH PTD* instead of playing is a delay.
	- If a player doesn't have *LH PTD*, playing the card known to be playable for the longest is a delay.
		- Note that this is not necessarily the rightmost card.
- The unlock target shifts 1 card to the left for every delay, following the *Unlock Promise* precedence rules.

### Locked Direct Discard Clues
- Sometimes, the best move in a locked situation is to discard a 4 that is far from being playable.
- When a clue is given to a locked player that reveals a 2-away or farther non-critical 4, the intent is for the locked player to discard the 4.
