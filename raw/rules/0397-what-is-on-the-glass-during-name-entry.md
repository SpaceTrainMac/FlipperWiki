---
rule: 0397
title: What is on the glass
source: FlipperEngine/docs/states/highscore.md § HighscoreMachine — What is on the glass
as-of: 0e97ce3
body: game
supersedes:
---
[highscore.md § HighscoreMachine — What is on the glass](../../../FlipperEngine/docs/states/highscore.md#what-is-on-the-glass)

| What | Where | Shows |
|---|---|---|
| the name being entered | that player's 6-digit score display | the confirmed characters, the one being edited, blanks after it |
| the other players' scores | their own displays | untouched, as `Play` left them |
| the place being recorded | `MATCH` (158) | `1ST`, `2ND` … `10TH`, right-aligned — or `NOSAVE` |
| whose turn | `FDLA_LED_ACTIVE_PLR_1..4` | one lit, all four written on every change |
| what this state is | `FDLA_LED_HIGH_SCORE` (177) | lit for the whole state, out on the way out |
