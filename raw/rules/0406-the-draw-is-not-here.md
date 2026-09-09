---
rule: 0406
title: The end-of-game draw is not here
source: FlipperEngine/docs/states/highscore.md § HighscoreMachine — What this state does not do
as-of: 0e97ce3
body: game
supersedes:
---
[highscore.md § HighscoreMachine — What this state does not do](../../../FlipperEngine/docs/states/highscore.md#what-this-state-does-not-do)

- **The end-of-game draw is not here.** It belongs to `PlayMachine` and is over — number read, display
  blanked — before this state opens ([the end-of-game draw](../../../FlipperEngine/docs/states/draw.md)). This state's obligation to
  `MATCH` is unchanged: it writes the place while somebody is typing and blanks it on the way out.
