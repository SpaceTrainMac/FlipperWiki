---
rule: 0250
title: A failed write is not renamed over a good file
source: FlipperEngine/docs/cabinet.md § 1. The settings file
as-of: 0e97ce3
body: cabinet
supersedes:
---
[cabinet.md § 1. The settings file](../../../FlipperEngine/docs/cabinet.md#1-the-settings-file)

- **A failed write is not renamed over a good file.** All three writers here test the stream after
  writing and delete the temp instead of renaming it — `highscores.csv` only since 2026-09-01,
  where a card that filled mid-table used to put the truncated file over the only copy of a table
  that exists nowhere else
  ([20260831-audit-fixes.md §3](../../../FlipperEngine/docs/concepts/done/20260831-audit-fixes.md#3-the-data-loss-writer-gets-its-red-first-test)).
  `NOSAVE` on the glass is what that failure looks like.
