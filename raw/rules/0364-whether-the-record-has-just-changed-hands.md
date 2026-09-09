---
rule: 0364
title: Whether the record has just changed hands
source: FlipperEngine/docs/states/game.md § GameMachine — The high score announcement
as-of: 0e97ce3
body: game
supersedes:
---
[game.md § GameMachine — The high score announcement](../../../FlipperEngine/docs/states/game.md#the-high-score-announcement)

The end of `processGameplay()` reports the running score to `HighScoreManager`, which holds the game
in progress as well as the table, and gets back the one thing an instantaneous comparison cannot
answer: **whether the record has just changed hands.** A table alone cannot answer it, because the
table cannot move while a game is running — so a second player passing the *old* top row would set
the knocker off while they were half a million behind the person standing next to them.
