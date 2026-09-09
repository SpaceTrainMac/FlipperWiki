---
rule: 0413
title: Two rows of twelve characters
source: FlipperEngine/docs/states/credits.md § CreditsMachine — What is displayed
as-of: 0e97ce3
body: game
supersedes:
---
[credits.md § CreditsMachine — What is displayed](../../../FlipperEngine/docs/states/credits.md#what-is-displayed)

**Two rows of twelve characters**, which is the four player score displays taken as one span
([hardware.md §2](../../../FlipperArchitecture/docs/hardware.md#2-displays-7-segment)):

| Row | Displays | Shows | Action | Speed |
|---|---|---|---|---|
| top | PLR_1, PLR_2 | the contributors, one string, for the whole state | `ActionDisplayMarqueeLoop` | `MARQUEE_SLOW`, 400 ms/char |
| bottom | PLR_3, PLR_4 | one quote, then the next one | `ActionDisplayMarquee`, one per quote | `MARQUEE_NORMAL`, 200 ms/char |
| the fifth display | MATCH | `CRDTS`, still, for the whole state | `ActionDisplaySpan`, written once | — |
