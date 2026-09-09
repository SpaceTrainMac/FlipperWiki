---
rule: 0384
title: It is a decision point, not a screen
source: FlipperEngine/docs/states/highscore.md § HighscoreMachine — recording the scores
as-of: 0e97ce3
body: game
supersedes:
---
[highscore.md § HighscoreMachine — recording the scores](../../../FlipperEngine/docs/states/highscore.md#highscoremachine--recording-the-scores)

**It is a decision point, not a screen.** On most games it does nothing at all and returns in under a
millisecond: a cabinet played for a week has ten rows that are hard to beat, and a decision point
that has decided *no* has nothing to say. The state after it is a minute of closing titles, and that
is where a game's ending belongs.
