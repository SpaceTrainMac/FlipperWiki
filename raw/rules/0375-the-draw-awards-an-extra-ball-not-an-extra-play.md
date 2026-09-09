---
rule: 0375
title: Decided 2026-08-19: it awards an extra ball, not an extra play
source: FlipperEngine/docs/states/draw.md § The end-of-game draw
as-of: 0e97ce3
body: game
supersedes:
---
[draw.md § The end-of-game draw](../../../FlipperEngine/docs/states/draw.md#the-end-of-game-draw)

**Decided 2026-08-19: it awards an extra ball, not an extra play.** The hardware distinguishes the
two — `FDLA_LED_EXTRA_PLAY` (175) and `FDLA_DISP1_EXTRA_PLAYS` (152) are a free *game* and a counter
of games owed — but credits are out of scope on a cabinet played at home
([`PlayerSelect`](../../../FlipperEngine/docs/states/player-select.md)), so an award of *extra play* has nowhere
to go and a ball has. `FDLA_LED_MATCH` (179) lights when the draw hits; the two extra-ball lamps
(174 / 176) are the playfield's and are not touched here.
