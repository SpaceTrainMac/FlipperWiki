---
rule: 0402
title: The table is written after every name, and a failed write is not the error state
source: FlipperEngine/docs/states/highscore.md § HighscoreMachine — The table is written after every name
as-of: 0e97ce3
body: game
supersedes:
---
[highscore.md § HighscoreMachine — The table is written after every name](../../../FlipperEngine/docs/states/highscore.md#the-table-is-written-after-every-name)

`HighScoreManager::store()` is crash-safe — a temp file and a `rename(2)` — so four names cost four
renames and buy the property that a power cut after the second player keeps the first two. **A failed
write is not the `ERROR` state**: `NOSAVE` goes on `MATCH` in place of the place and the state
carries on, because a cabinet that cannot save a name still plays pinball and will simply have
forgotten by morning ([guidelines.md §4](../../../FlipperEngine/docs/guidelines.md#4-error-handling)).
