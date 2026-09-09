---
rule: 0374
title: The ball it awards is an ordinary turn
source: FlipperEngine/docs/states/draw.md § The end-of-game draw
as-of: 0e97ce3
body: game
supersedes:
---
[draw.md § The end-of-game draw](../../../FlipperEngine/docs/states/draw.md#the-end-of-game-draw)

**The ball it awards is an ordinary turn**, taken in player order like any other: the playfield is
reset on entry the way it is at the start of every turn, and `BALL IN PLAY` simply counts on. Nothing
about it is special once the loop has resumed.
