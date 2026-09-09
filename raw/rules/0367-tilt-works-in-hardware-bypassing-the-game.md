---
rule: 0367
title: It works the same way the flippers do: in hardware, bypassing the game logic entirely
source: FlipperEngine/docs/states/game.md § GameMachine — Tilt is not a host concern
as-of: 0e97ce3
body: game
supersedes:
---
[game.md § GameMachine — Tilt is not a host concern](../../../FlipperEngine/docs/states/game.md#tilt-is-not-a-host-concern)

It works the same way the flippers do: **in hardware, bypassing the game logic entirely.** On tilt
the machine kills its outputs and keeps them off until the balls have left the playfield. The host is
not consulted and cannot veto it — which is the right design, since a tilt must work whether or not
the Pi is healthy.

What the host *does* see is the aftermath: the ball drains, `BALLSENSOR_BALLCACHE` fires, and the
ball ends through the ordinary path. So the game logic needs no tilt handling to stay correct.
