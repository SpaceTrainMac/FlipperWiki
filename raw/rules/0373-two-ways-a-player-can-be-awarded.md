---
rule: 0373
title: There are two ways a player can be awarded, and this state owns the second
source: FlipperEngine/docs/states/draw.md § The end-of-game draw
as-of: 0e97ce3
body: game
supersedes:
---
[draw.md § The end-of-game draw](../../../FlipperEngine/docs/states/draw.md#the-end-of-game-draw)

There are **two** ways a player can be awarded, and this state owns the second:

1. **During play — `GameMachine` decides.** A `src/games/` class raises `SE_EXTRA_BALL` or
   `SE_FREE_BALL`, `GameMachine` sets the matching flag, and the self-transition above fires.
2. **At the end of the game — the draw.** Once every player is out of balls, `DrawMachine` puts a
   random number on `FDLA_DISP6_SCORE_MATCH` (158) and **every player whose score ends in those
   digits is handed one more ball**. The second round then plays whatever it awarded, which may be
   nothing.
