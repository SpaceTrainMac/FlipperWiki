---
rule: 0404
title: The announcement during a ball is not this state's
source: FlipperEngine/docs/states/highscore.md § HighscoreMachine — What this state does not do
as-of: 0e97ce3
body: game
supersedes:
---
[highscore.md § HighscoreMachine — What this state does not do](../../../FlipperEngine/docs/states/highscore.md#what-this-state-does-not-do)

- **The announcement during a ball is not this state's.** The `HIGH SCORE` lamp and the knocker fire
  from `GameMachine` the moment the best score on the cabinet changes hands, which is a question
  about a game in progress ([`GameMachine`](../../../FlipperEngine/docs/states/game.md)). `HighScoreManager` holds the
  running game so that it can be asked at all, and the knocker is latched to once per player per game
  and gated by a `knocker` key in settings.json.
