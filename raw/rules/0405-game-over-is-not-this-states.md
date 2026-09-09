---
rule: 0405
title: GAME OVER is not this state's
source: FlipperEngine/docs/states/highscore.md § HighscoreMachine — What this state does not do
as-of: 0e97ce3
body: game
supersedes:
---
[highscore.md § HighscoreMachine — What this state does not do](../../../FlipperEngine/docs/states/highscore.md#what-this-state-does-not-do)

- **`FDLA_LED_GAME_OVER` (167) is not this state's.** It names the end of a *game*, which is
  something `PlayMachine` knows and this state only inherits
  ([`GameOverMachine`](../../../FlipperEngine/docs/states/game-over.md)).
