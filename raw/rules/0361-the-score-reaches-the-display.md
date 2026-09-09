---
rule: 0361
title: The score reaches the display
source: FlipperEngine/docs/states/game.md § GameMachine — The score on the glass, and the playfield between turns
as-of: 0e97ce3
body: game
supersedes:
---
[game.md § GameMachine — The score on the glass, and the playfield between turns](../../../FlipperEngine/docs/states/game.md#the-score-on-the-glass-and-the-playfield-between-turns)

- **The score reaches the display.** `showScore()` writes `m_DISP6_SCORE_PLR`, from `initNewRound()`
  and from the one place the score changes — **on change rather than every cycle**, because a display
  command costs ~3 ms of pacing behind a slow µC. `PlayMachine` calls it once per player when it
  builds them, so every player reads `0` from the first ball rather than whatever the state before
  them left on the glass.
