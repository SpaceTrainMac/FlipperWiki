---
rule: 0371
title: It goes out because a ball is in play
source: FlipperEngine/docs/states/game-over.md § GAME OVER is this state's lamp
as-of: 0e97ce3
body: game
supersedes:
---
[game-over.md § GAME OVER is this state's lamp](../../../FlipperEngine/docs/states/game-over.md#game-over-is-this-states-lamp-and-the-turns-edge-is-its-counterpart)

**It goes out because a ball is in play**, in `GameMachine::beginTurn()` — not on the way into
`PlayMachine::run()`. That gives the lamp the same two-writer shape `AR_NO_PADDLE_MODE` has, and the
clearing rule it needs — `Credits` → `PlayerSelect` is a route into a game that passes nothing which
would clear it — then holds by construction rather than by a line somebody has to remember. It costs
one lamp write per turn, at most twelve a game.
