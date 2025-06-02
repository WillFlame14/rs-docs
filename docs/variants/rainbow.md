---
sidebar_position: 1
---

import useBaseUrl from '@docusaurus/useBaseUrl';

# Rainbowish

These apply to variants with a suit that is touched by all colours, such as Rainbow or Omni.

### Rainbow Promise
- When a rainbow card can be the *Focus* of a *Referential Play Clue* targeting slot 1, there is *Free Choice* to clue any colour.
- We promise that the card (if rainbow) is the rank matching the colour, with the rightmost colour matching the highest rank and shifting to the left, similar to a [*Mud Clue*](https://hanabi.github.io/variant-specific/muddy-rainbow-cocoa-rainbow#mud-clues).
	- For example, in a 5 suit Rainbow game:
		- Blue would promise m5/m1,
		- Green would promise m4,
		- Yellow would promise m3, and 
		- Red would promise m2.
- For *Referential Play Clues* that don't target slot 1, nothing is promised.
	- This is because it can be difficult to determine if there was *Free Choice* or not.

<figure>
    <img src={useBaseUrl('/img/rainbow-promise.png')} alt="Alice's slots 2, 4 and 5 are previously clued. Bob clues blue to Alice, touching slots 2 and 3." width="100%"/>
    <figcaption>This promises Alice's slot 3 to either be a blue card, m1 or m5. She would write a note of [b,m1,m5].</figcaption>
</figure>