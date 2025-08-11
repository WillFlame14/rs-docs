---
sidebar_position: 4
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Level 5 - Exceptional Situations

## Stalling Situations

- A player is in a stalling situation if they are forced to give a clue. The following are examples of stalling situations:
  - Turn 1
  - At 8 clues

There are special rules around being *Locked* that are covered in [level 4](./level-4).

### Starting Hand Stalls
- On turn 1, if Alice clues a rank clue touching slot 5, this is a *Starting Hand Stall* and Bob is forced into a stalling situation.
  - If Alice doesn't immediately follow up with another clue, Bob has *Permission to Discard* slot 1.
- This does not apply if Alice clues a *Playable Rank Clue*, such as 1.

### Rank Stalls
- *Reclues* and *Lock Clues* are interpreted as stalls.
- *Playable Rank Clues* and *Referential Discard Clues* are the same as while unlocked.
- [*Loaded Rank Play Clues*](./level-3#loaded-rank-play-clues) are interpreted as *Referential Discard Clues*.

Every other clue is interpreted normally.

## Emergency Situations

### Zero Clue Safety Promise
- When Alice uses the last clue, she promises a safe discard in Bob's hand, referred to as *ZCSP*.
    - From highest to lowest priority, the possible targets are known trash, leftmost unclued and not [*Chop Moved*](./level-3#chop-moves), and least likely to be critical.
    - A card with *ZCSP* is considered to be known trash, and the player is *Loaded* until it is discarded.
- If all of Bob's cards are critical, Bob is not promised a safe discard.
    - This is a very dangerous situation, and if Alice is unable to give Bob an *Extra Discard* as shown below, Bob should use his best judgement in deciding what to discard (likely the newest drawn card).

<figure>
    <img src={useBaseUrl('/img/zcsp.png')} alt="Alice uses the last clue to fill in a playable r5. Bob's slots 1 and 2 are unclued." width="100%"/>
    <figcaption>Alice uses the last clue to fill in a playable r5. Since this clue *Chop Moves* slot 1, slot 2 is promised to be *ZCSP*.</figcaption>
</figure>

### Zero Clue Free Choice Extra Discard
- **At 0 clues**, if Alice can choose between regaining a clue and not, staying at zero clues promises Bob's slot 1 to be trash as an *Extra Discard*.
    - As a corollary, gaining a clue (by discarding or playing a 5) causes a [*Scream Discard Chop Move*](./level-3#chop-moves) on slot 1.
    - If Alice can only choose between playing a 5 or discarding, playing the 5 promises Bob's slot 1 to be trash.
- Giving Bob an *Extra Discard* may allow Bob to have *Free Choice* to give Alice an *Extra Discard* as well.
- If the clue count is above 0, choosing to play over discard has no extra meaning.

In the example in the previous section, since Bob can discard *ZCSP* in slot 2, playing r5 gives Alice an *Extra Discard* in slot 1.
  - Normally, it would be automatically sieved after Alice plays her known y2.

### Bomb Lock
- Bombing known trash (including *PTD* or *ZCSP*) locks the other player.

### Scream Lock
- Discarding chop or known trash while having a globally known playable (outside of *SDCMs* at 0 clues) locks the other player.

### Sacrifice Unlock
- Sacrificing a card to unlock yourself can only be done immediately after being locked. This does not promise a *Baton* or [*Gentleman's Discard*](./level-6#gentlemans-discard).
  - Occasionally, the team's best discard is an uncritical 4 in the locked player's hand. This would be a good time to perform a *Sacrifice Unlock*.

### Sacrifice Scream Lock
- If a *Sacrifice Discard* is performed multiple turns after being locked, this locks the other player.

## Rationale

- Because we don't have information about future chops, it's possible that saving one card can lead to additional criticals or 5s being drawn after discarding.
  - Thus, it's often better to lock a hand with low, useful cards like 3s and 4s than to save individual cards and potentially end up drawing high, critical cards.
  - The multiple ways to lock above facilitate these techniques while maintaining a healthy clue count.
