---
rule: 0417
title: The names scroll at half the speed of the quotes
source: FlipperEngine/docs/states/credits.md § CreditsMachine — What is displayed
as-of: 0e97ce3
body: game
supersedes:
---
[credits.md § CreditsMachine — What is displayed](../../../FlipperEngine/docs/states/credits.md#what-is-displayed)

**The names scroll at half the speed of the quotes**, and both numbers follow from what the row has
to say. The top row is three names going round for the whole state, so it can be read at a stroll. A
quote is one pass of up to 120 characters across a 12-character span, and the roll only lasts a
minute: at `MARQUEE_SLOW` the longest one would take 53 seconds — nearly the entire default duration
for a single sentence — against 26 at `MARQUEE_NORMAL`, which leaves room for a second quote and, on
the short ones, a third.
