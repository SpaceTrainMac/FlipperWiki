---
rule: 0370
title: GAME OVER names the end of a game, and Play is the only state that decides that
source: FlipperEngine/docs/states/game-over.md § GAME OVER is this state's lamp
as-of: 0e97ce3
body: game
supersedes:
---
[game-over.md § GAME OVER is this state's lamp](../../../FlipperEngine/docs/states/game-over.md#game-over-is-this-states-lamp-and-the-turns-edge-is-its-counterpart)

`FDLA_LED_GAME_OVER` (167) names the end of a *game*, and `Play` is the only state that knows when
that is: the states after it inherit the fact rather than establishing it
([20260819-highscore-entry.md §12.4](../../../FlipperEngine/docs/concepts/done/20260819-highscore-entry.md#124-nobody-lights-game-over)).
`GameOverMachine` lights it when the last round ends.
