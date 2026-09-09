---
rule: 0383
title: Entered whenever Play finishes, unconditionally
source: FlipperEngine/docs/states/highscore.md § HighscoreMachine — recording the scores
as-of: 0e97ce3
body: game
supersedes:
---
[highscore.md § HighscoreMachine — recording the scores](../../../FlipperEngine/docs/states/highscore.md#highscoremachine--recording-the-scores)

Entered whenever `Play` finishes, **unconditionally**, and it leaves to
[`Credits`](../../../FlipperEngine/docs/states/credits.md), unconditionally. Whether anyone actually earned
a place is decided inside this state, which passes straight through when nobody did. Keeping that
test here rather than on the transition means only one piece of code knows what "qualifies" means.
