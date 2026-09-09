---
rule: 0346
title: All button handling is edge-triggered
source: FlipperEngine/docs/states/player-select.md § PlayerSelect — choosing the number of players
as-of: 0e97ce3
body: game
supersedes:
---
[player-select.md § PlayerSelect — choosing the number of players](../../../FlipperEngine/docs/states/player-select.md#playerselect--choosing-the-number-of-players)

**All button handling is edge-triggered**, which is what makes reusing `START` safe. The sensor layer
reports *changes*, not levels: `SensorField::isSensorTriggeredHigh` only
answers true for a switch that became active **in this update**. One physical press is one rising
edge, consumed once — holding the button down produces nothing further, and STM32-IN sends no frame
at all while a button is merely held.

So the press that leaves `Intro` cannot also commit in `PlayerSelect`. No release-detection or
debounce logic is needed at this level.
