---
rule: 0385
title: The merge is the test
source: FlipperEngine/docs/states/highscore.md § HighscoreMachine — Who qualifies
as-of: 0e97ce3
body: game
supersedes:
---
[highscore.md § HighscoreMachine — Who qualifies](../../../FlipperEngine/docs/states/highscore.md#who-qualifies)

**The merge is the test**, and it is answered once, on entry, by
`HighScoreManager::qualifyingPlaces()`: the table as it stands, plus the game's scores appended in
player order, sorted and trimmed to ten. A player qualifies if and only if their row survives, and
their place is the row it is standing in — deliberately **the same arithmetic `addHighScore()`
performs later**, so the place on the glass and the table on disk are one calculation rather than two
that have to be kept in agreement.
