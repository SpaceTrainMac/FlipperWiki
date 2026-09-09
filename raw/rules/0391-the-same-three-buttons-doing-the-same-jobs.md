---
rule: 0391
title: Same three buttons doing the same three jobs
source: FlipperEngine/docs/states/highscore.md § HighscoreMachine — Name entry
as-of: 0e97ce3
body: game
supersedes:
---
[highscore.md § HighscoreMachine — Name entry](../../../FlipperEngine/docs/states/highscore.md#name-entry)

Same three buttons doing the same three jobs as [`PlayerSelect`](../../../FlipperEngine/docs/states/player-select.md)
and [`Setup`](../../../FlipperEngine/docs/states/setup.md), which is why there is one interaction model on this machine
and not three. **Auto-repeat is not optional** — the sensor field reports one edge however long a
button is held — and it lives in `RepeatingButton`, shared with the service menu.
