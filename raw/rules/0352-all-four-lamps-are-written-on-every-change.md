---
rule: 0352
title: All four lamps are written on every change, not just the one that moved
source: FlipperEngine/docs/states/player-select.md § PlayerSelect — choosing the number of players
as-of: 0e97ce3
body: game
supersedes:
---
[player-select.md § PlayerSelect — choosing the number of players](../../../FlipperEngine/docs/states/player-select.md#playerselect--choosing-the-number-of-players)

**All four lamps are written on every change, not just the one that moved.** Stepping down from
three to two has to put a lamp *out*, and a draw that only ever lights things cannot — four commands
on a keypress is nothing next to getting that wrong in the direction nobody tests.
