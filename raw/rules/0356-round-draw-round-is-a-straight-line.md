---
rule: 0356
title: Round to draw to round is a straight line, not a loop
source: FlipperEngine/docs/states/play.md § PlayMachine — inside the Play state
as-of: 0e97ce3
body: game
supersedes:
---
[play.md § PlayMachine — inside the Play state](../../../FlipperEngine/docs/states/play.md#playmachine--inside-the-play-state)

**Round → draw → round is a straight line, not a loop**, and that is what makes *the draw happens
once* structural rather than a flag: a second draw cannot run because a second draw is not written.
The `m_drawSpent` boolean the old shape needed is gone with the loop that needed it.
