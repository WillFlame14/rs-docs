---
sidebar_position: 1
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Level 2 - Reclues

- When a clue touches no new cards, it is called a **reclue**. A reclue that reveals a playable or trash card has no additional meaning.
- But what if no safe action is revealed? Such a clue should be interpreted as intending the focused card to be playable, promising playable cards in the hand.
	- The *Focus* of a reclue is the leftmost touched card.

## Special Moves

### The Prompt

- When there are clued cards that could connect to the card, the **rightmost** such card is promised to connect.
    - Connecting cards can match in either rank or colour.
- This is called a *Prompt*, since it is like the card is being "prompted" to play.

<figure>
    <img src={useBaseUrl('/img/prompt.png')} alt="b1 is on the play stacks. Alice clues 3 to Bob, filling in b3. Bob has two other blue cards on slots 2 and 3." width="100%"/>
    <figcaption>Alice is prompting Bob's slot 3 to play as b2.</figcaption>
</figure>

### The Finesse

- If there are no clued cards that could connect, the **leftmost unclued card** (usually slot 1) is promised to connect.
- This is called a *Finesse*, like the term in bridge.

<figure>
    <img src={useBaseUrl('/img/finesse.png')} alt="b1 is on the play stacks. Alice clues 3 to Bob, filling in b3. Bob has no other blue cards." width="100%"/>
    <figcaption>Alice is finessing Bob's slot 1 to play as b2.</figcaption>
</figure>

### The Bluff

- It is not required that the blind-played card actually connects to the *Focus* in a *Finesse*, as long as it is playable.
- If the card does not connect, this is known as a *Bluff*.
- After the blind play of an unconnected card, the receiver will know that a *Bluff* occurred and stop playing.

<figure>
    <img src={useBaseUrl('/img/bluff.png')} alt="b1 is on the play stacks. Alice clues 3 to Bob, filling in b3. Bob plays slot 1 as a finesse, but it turns out to be r1." width="100%"/>
    <figcaption>Alice *Bluffed* Bob's slot 1, getting r1 to play. Bob is not promised b2 anywhere.</figcaption>
</figure>

### The No-Info Double Bluff

- If a reclue is given that does not fill in the focused card (gives no new information), this is very strange.
- Normally, a clue is used to fully reveal the card, so the receiver can tell if it's playable, trash, or needs connecting cards.
- But since this clue is so useless, it gets **the two leftmost unclued cards** to play as a *Double Bluff*.
	- Nothing is promised about the focus.

<figure>
    <img src={useBaseUrl('/img/no-info-db.png')} alt="Alice clues blue to Bob, not touching any new cards or filling in any cards." width="100%"/>
    <figcaption>Alice intends to *Double Bluff* Bob's slot 1 and slot 2.</figcaption>
</figure>

- A *No-Info Double Bluff* can be performed on cards that are already fully known, even known trash.
- The only requirement is that the clue gives no new information about any touched cards.

## Conventions

### Precedence Between Prompts and Finesses

- If the focus is more than 1-away from playable, it is ambiguous whether to play into a *Prompt* or a *Finesse*.
- If it is possible that no *Finesses* are required, only *Prompts*, then this is the preferred interpretation.
- If at least one blind play would be required, it should be performed first.
    - If the blind-played card doesn't connect, this becomes a *Bluff* and the receiver isn't promised anything else.
