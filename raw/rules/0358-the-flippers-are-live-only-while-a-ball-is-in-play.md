---
rule: 0358
title: The flippers are live for exactly as long as a ball is on the playfield
source: FlipperEngine/docs/states/play.md § PlayMachine — The flippers are dead between turns
as-of: 0e97ce3
body: game
supersedes:
---
[play.md § PlayMachine — The flippers are dead between turns](../../../FlipperEngine/docs/states/play.md#the-flippers-are-dead-between-turns)

**The flippers are live for exactly as long as a ball is on the playfield.**
`GameMachine::beginTurn()` disarms `AR_NO_PADDLE_MODE` and `endTurn()` arms it again, so every gap
between turns is dead — including the 3000 ms the draw is read in, which is the longest of them and
the only one anybody would notice.
