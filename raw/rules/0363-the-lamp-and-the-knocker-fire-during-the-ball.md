---
rule: 0363
title: The lamp and the knocker fire from here, not from HighscoreMachine
source: FlipperEngine/docs/states/game.md § GameMachine — The high score announcement
as-of: 0e97ce3
body: game
supersedes:
---
[game.md § GameMachine — The high score announcement](../../../FlipperEngine/docs/states/game.md#the-high-score-announcement)

**The lamp and the knocker fire from here, not from [`HighscoreMachine`](../../../FlipperEngine/docs/states/highscore.md).**
The two states ask different questions and that is the whole distinction: the announcement asks *has
this player just taken the best score on the cabinet*, about a ball in progress, and the recording
asks *which of these four scores belong in the table*, about a game that has finished.
