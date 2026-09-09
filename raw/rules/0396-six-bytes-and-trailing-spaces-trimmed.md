---
rule: 0396
title: Six bytes, NUL-padded
source: FlipperEngine/docs/states/highscore.md § HighscoreMachine — Name entry
as-of: 0e97ce3
body: game
supersedes:
---
[highscore.md § HighscoreMachine — Name entry](../../../FlipperEngine/docs/states/highscore.md#name-entry)

**Six bytes, NUL-padded**, which is the convention the table already has. Trailing spaces become NUL
on commit and only the trailing ones — `MR T` is three letters and a gap and survives whole.
