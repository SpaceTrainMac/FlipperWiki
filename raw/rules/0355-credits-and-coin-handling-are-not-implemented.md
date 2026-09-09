---
rule: 0355
title: Scope decision: credits and coin handling are not implemented and not planned
source: FlipperEngine/docs/states/player-select.md § PlayerSelect — choosing the number of players
as-of: 0e97ce3
body: game
supersedes:
---
[player-select.md § PlayerSelect — choosing the number of players](../../../FlipperEngine/docs/states/player-select.md#playerselect--choosing-the-number-of-players)

> **Scope decision: credits and coin handling are not implemented and not planned**, even though the
> cabinet has the hardware for them — `FDLA_LED_CREDITS` (178), `FDLA_DISP2_CREDITS` (156),
> `FDLA_DISP1_EXTRA_PLAYS` (152), `FDLA_LED_EXTRA_PLAY` (175). The machine is played at home, not
> coin-operated.
>
> **Nothing to do with the `Credits` state** ([`CreditsMachine`](../../../FlipperEngine/docs/states/credits.md)), which
> is the roll of names at the end of a game and touches none of those four addresses. One word, two
> meanings, and only the closing-titles one is built.
