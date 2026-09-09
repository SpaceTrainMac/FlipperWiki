---
rule: 0351
title: Showing the count, in two places at once
source: FlipperEngine/docs/states/player-select.md § PlayerSelect — choosing the number of players
as-of: 0e97ce3
body: game
supersedes:
---
[player-select.md § PlayerSelect — choosing the number of players](../../../FlipperEngine/docs/states/player-select.md#playerselect--choosing-the-number-of-players)

**Showing the count, in two places at once.** The status row's left-hand digit,
`FDLA_DISP1_EXTRA_PLAYS` (152), carries the number, and the four player-active indicators —
`FDLA_LED_ACTIVE_PLR_1..4` (164, 165, 169, 171) — light one through four beside it. The digit *says*
the count and the lamps *show* it, which are the two places a player already looks during a game.

That digit is free here for the same reason `BALL_IN_PLAY` is: no ball is in play and no extra plays
have been won in a game that has not started. `Play` takes the status row over on the way out.
