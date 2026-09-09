---
rule: 0412
title: Both ends of the range are clamped and warned rather than refused
source: FlipperEngine/docs/states/credits.md § CreditsMachine — The duration is configuration, not a constant
as-of: 0e97ce3
body: game
supersedes:
---
[credits.md § CreditsMachine — The duration is configuration, not a constant](../../../FlipperEngine/docs/states/credits.md#the-duration-is-configuration-not-a-constant)

Both ends of the range are real mistakes to make by hand, so the value is **clamped and warned about
rather than refused**, exactly as a volume of 150 is: a zero would make the state a flicker nobody
can read, and a value in days would park the cabinet in it looking broken.
