---
rule: 0395
title: The first ring position is a rub-out
source: FlipperEngine/docs/states/highscore.md § HighscoreMachine — Name entry
as-of: 0e97ce3
body: game
supersedes:
---
[highscore.md § HighscoreMachine — Name entry](../../../FlipperEngine/docs/states/highscore.md#name-entry)

**The first ring position is a rub-out** (`DISPLAY_CHAR_BAR`, the left-hand upright): `START` on it
moves *back* one character, discards what was there, and stays on the rub-out — so a held button
walks back through the whole name and stops dead at the first character, where it does nothing.
`START` auto-repeats there and **nowhere else**: held on a character it would finish a name before
the player let go.
