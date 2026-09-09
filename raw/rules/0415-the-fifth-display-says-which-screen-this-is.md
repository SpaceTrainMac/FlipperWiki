---
rule: 0415
title: The fifth display says which screen this is
source: FlipperEngine/docs/states/credits.md § CreditsMachine — What is displayed
as-of: 0e97ce3
body: game
supersedes:
---
[credits.md § CreditsMachine — What is displayed](../../../FlipperEngine/docs/states/credits.md#what-is-displayed)

**The fifth display says which screen this is**, because the other two rows never stand still:
somebody who walks up mid-quote can otherwise watch a sentence go past without learning what they are
looking at. It is written once on the first cycle and blanked with everything else on the way out —
nothing in this state touches MATCH, so what is put there stays there. `CRDTS` rather than `CREDITS`
because a 6-digit group holds six characters, and it is [not the coin
sense](../../../FlipperEngine/docs/states/credits.md#58-creditsmachine--the-closing-titles) of the word either way.
