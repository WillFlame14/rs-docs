---
sidebar_position: 3
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Level 4 - Locked Hands

- A player is *Locked* after they receive a [*Lock Clue*](../basics/discard-clues#lock-clues), and cannot discard any cards until further information is given.
- While they are *Locked*, the types of clues they can give are restricted so that they can be unlocked efficiently.
- When pace is greater than 2, it is better for the unlocked player to discard instead of playing a card that doesn't connect to one of the locked player's cards.
	- Thus, it is important that the unlocked player has full information about their playable cards.

## Conventions

- Unlike H-Group, **being at 8 clues is not a special case of being locked**. Both are stalling situations, but they arise due to different circumstances and are thus handled differently.
	- At 8 clues, there are no *Colour Stalls*, but *Reclues* and *Lock Clues* are interpreted as stalls.

### Colour Clues While Locked

- Any colour clue not touching slot 1 is a *Colour Stall*.
- A colour clue that touches slot 1 means that slot 1 is playable.

<figure>
    <img src={useBaseUrl('/img/colour-stall.png')} alt="Alice is locked. She clues green to Bob, newly touching slot 1." width="100%"/>
    <figcaption>Alice is promising g1 in Bob's slot 1. This is not a *Referential Play Clue* on slot 3. Bob also has *LH PTD* on slot 2.</figcaption>
</figure>

### Rank Clues While Locked

- *Playable Rank Clues* and *Referential Discard Clues* are the same as while unlocked.
- [*Loaded Rank Play Clues*](./level-3#loaded-rank-play-clues) are interpreted as *Referential Discard Clues*.
- *Reclues* and *Lock Clues* are interpreted as stalls.

<figure>
    <img src={useBaseUrl('/img/rank-stall.png')} alt="Alice is locked. She clues 5 to Bob, newly touching slot 5." width="100%"/>
    <figcaption>Alice is stalling, giving *LH PTD* on Bob's slot 1.</figcaption>
</figure>

### Locked Hand PTD

- Except for *Playable Rank Clues*, every clue given by the locked player promises a safe discard: *Locked Hand PTD*.
	- For *Referential Discard Clues*, this is simply the card called to discard.
	- Otherwise (e.g. *Colour Stalls*, *Lock Clues*, colour clues touching slot 1), this is the leftmost unclued card.

- If every card in the unlocked player's hand becomes clued, they do not receive *LH PTD*.

### Unlock Promise

- If the unlocked player chooses to play a **commonly-known** card even when they have *Locked Hand PTD*, this promises that the locked player can become unlocked.
  - If the unlocked player plays a card whose identity is not commonly known, this does not promise an unlock.
- To determine how to unlock, the locked player should first try to connect in the same suit.
  - For example, if r3 was played, the locked player should try to prompt a card as r4.
- If no cards could connect, then they should try the card most likely to be playable, biasing rightmost.
- If the unlocked player could be trying to connect through multiple cards in their own hand (e.g. r3 and r4 to connect to r5), then the locked player should continue to stall.

<figure>
    <img src={useBaseUrl('/img/unlock-promise.png')} alt="Bob is locked, with an unknown card, a clued 4, g4, y5, and a clued 3. Alice has a known r1, unknown LH PTD, y3 and p2. The play stacks are at [0, 2, 2, 2, 1]." width="100%"/>
    <figcaption>Bob is locked, telling Alice about r1 in slot 1. Alice has multiple choices of playable cards, as well as *LH PTD* on slot 3.</figcaption>
</figure>

In the above example, Bob is locked. Alice has several options, each with different meanings:
- If Alice plays r1, Bob's slot 1 is promised to be r2 (or some other playable card).
- If Alice plays y3, Bob's slot 2 is promised to be y4.
- If Alice plays p2, Bob's slot 5 is promsied to be p3.
- If Alice discards slot 2 (*LH PTD*), Bob can write negative notes for all the above identities.

### Unlock Promise Shifting

- If the unlocked player chooses to delay before playing a connecting card, this causes the unlock target to shift.
- A **delay** is any action that is not forced. For example:
	- discarding *LH PTD* or known trash instead of playing
	- without trash, playing the card known to be playable for the longest (not necessarily the rightmost)
	- without trash, playing a playable card that has been delayed enough times to be known not to connect
- The unlock target shifts 1 card to the left for every delay, following the *Unlock Promise* precedence rules.

In the example in the previous section, if Alice discards *LH PTD* and then plays y3, Bob's slot 1 is promised to be y4.

### Locked Direct Discard Clues
- Sometimes, the best move in a locked situation is to discard a 4 that is far from being playable.
- When a clue is given to a locked player that reveals a 2-away or farther non-critical 4, the locked player should discard the 4.
