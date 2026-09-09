---
rule: 0372
title: Two consequences, both deliberate
source: FlipperEngine/docs/states/game-over.md § GAME OVER is this state's lamp
as-of: 0e97ce3
body: game
supersedes:
---
[game-over.md § GAME OVER is this state's lamp](../../../FlipperEngine/docs/states/game-over.md#game-over-is-this-states-lamp-and-the-turns-edge-is-its-counterpart)

Two consequences, both deliberate. A game with **zero players** no longer clears the lamp, because no
turn runs; `PlayerSelect` cannot produce one and the top level does not route one, so this is
reachable only from the isolated processes and the tests, and leaving it lit when no game was played
is the more honest answer. And a **shutdown** leaves the lamp untouched rather than written false:
nothing lights it, which is the guarantee, and the first ball of the next game puts out whatever the
last one left.
