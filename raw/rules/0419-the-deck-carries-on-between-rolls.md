---
rule: 0419
title: The deck carries on from one roll to the next
source: FlipperEngine/docs/states/credits.md § CreditsMachine — What is displayed
as-of: 0e97ce3
body: game
supersedes:
---
[credits.md § CreditsMachine — What is displayed](../../../FlipperEngine/docs/states/credits.md#what-is-displayed)

The deck **carries on from one roll to the next** rather than being dealt again by `run()`, so a
second game does not open with the quote the first one opened with. It is the only state in this
machine that outlives a `run()`.
