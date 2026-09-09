---
rule: 0399
title: How an entry ends
source: FlipperEngine/docs/states/highscore.md § HighscoreMachine — How an entry ends
as-of: 0e97ce3
body: game
supersedes:
---
[highscore.md § HighscoreMachine — How an entry ends](../../../FlipperEngine/docs/states/highscore.md#how-an-entry-ends)

| Exit | What is recorded |
|---|---|
| the sixth character confirmed | the six characters |
| `nameEntrySeconds` with no button at all | **what is on the glass** — the confirmed characters plus the one being edited |
| a shutdown request | the same commit |
