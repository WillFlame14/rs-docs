---
sidebar_position: 5
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Level 6 - Elimination

### Elimination Notes
- Certain cards are so important that they must always be saved in normal situations, and discarding them promises that the duplicate is elsewhere in the hand.
- These are known as *Elimination Notes*, which are slowly reduced as more information is learned.
- Elimination notes are **only written when**:
	- a delayed playable card (or 2) is called to discard
	- a delayed playable card (or 2) is given *Permission To Discard* while there were 2+ clues
- If elimination notes for a playable identity are reduced to a single card, even if it has 0 positive clues, that player is *Loaded* and is expected to play that card.
- Otherwise, elimination does not apply.

<figure>
    <img src={useBaseUrl('/img/elimination.png')} alt="Alice discards a playable r3 from slot 1, while having yellow clued in slot 3 and 4 clued in slots 4 and 5." width="100%"/>
    <figcaption>Alice discards a playable r3 from *PTD*, resulting in *Elimination Notes* for the second copy of r3 in slot 2. Alice is now *Loaded*.</figcaption>
</figure>

## Special Discards

### Sarcastic Discard

- Occasionally, multiple copies of an identity may end up between both players' hands.
- This is typically resolved by having the player who realizes the duplication first discard their copy.
- The other player is promised to have the duplicate, but it could be anywhere except chop (it may not even be clued).
	- The exception is when the discarded card is playable, which is referred to as a *Gentleman's Discard* and described below.

### Gentleman's Discard
- When a playable card is discarded, the duplicate is promised in partner's rightmost possible position.
	- If the duplicate is not in the rightmost position, the card **cannot be discarded**, or a bomb will occur.
	- The exception is when a *Layered Gentleman's Discard* is performed, described below.

<figure>
    <img src={useBaseUrl('/img/bad-gd.png')} alt="Alice has a clued b3 and a clued b5, while Bob has a known playable b3." width="100%"/>
    <figcaption>Bob **cannot** perform a *Gentleman's Discard* by discarding b3, otherwise Alice will bomb b5.</figcaption>
</figure>

### Layered Gentleman's Discard
- A *Gentleman's Discard* can be performed even if the duplicate isn't in the rightmost position as long as **all possible positions until the duplicate** (from the right) are playable.
- This is known as a *Layered Gentleman's Discard*, since the duplicate is layered behind the other playable cards.

<figure>
    <img src={useBaseUrl('/img/layered-gd.png')} alt="Bob has a playable g4. Alice has a playable g4 and p2 in slots 3 and 4, with a clued b2 in slot 5." width="100%"/>
    <figcaption>Bob can perform a *Layered Gentleman's Discard* discarding g4, which causes Alice to play p2 and then g4.</figcaption>
</figure>

### Trash Order Chop Move

- This is [a similar convention to the one in H-Group](https://hanabi.github.io/level-14#the-trash-order-chop-move-tocm), but not the same.
- Known trash should be discarded from **right-to-left**.
