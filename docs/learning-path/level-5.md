---
sidebar_position: 4
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Level 5 - Emergency Situations

## Conventions

### Zero Clue Safety Promise
- When Alice uses the last clue, she promises at least one safe discard in Bob's hand (referred to as *ZCSP*).
	- From highest to lowest priority, the possible targets are known trash, leftmost unclued and not [*Chop Moved*](./level-3#chop-moves), and least likely to be critical.
- When Alice uses the last clue and all of Bob's cards are critical, Bob's next draw is *ZCSP*.

### Zero Clue Free Choice Extra Discard
- At 0 clues, if Alice has free choice between playing and discarding trash (including *PTD* or *ZCSP*), playing promises Bob's slot 1 to be trash.
- This can give Bob *Free Choice* to give Alice an *Extra Discard* as well.

### Bomb Lock
- Bombing a card with *PTD* or bombing known trash locks the other player.

### Scream Lock
- Discarding chop or known trash while having a globally known playable (outside of *SDCMs* at 0 clues) locks the other player.

### Sacrifice Unlock
- Sacrificing a card to unlock yourself can only be done immediately after being locked. This does not promise a *Baton* or *Gentleman's Discard* (introduced at level 6).
  - Occasionally, the team's best discard is an uncritical 4 in the locked player's hand. This would be a good time to perform a *Sacrifice Unlock*.

### Sacrifice Scream Lock
- If a *Sacrifice Discard* is done not immediately after being locked, this locks the other player.

## Rationale

- Because we don't have information about future chops, it's possible that saving one card can lead to additional criticals or 5s being drawn after discarding.
  - Thus, it's often better to lock a hand with low, useful cards like 3s and 4s than to save individual cards and potentially end up drawing high, critical cards.
  - The multiple ways to lock above facilitate these techniques while maintaining a healthy clue count.
