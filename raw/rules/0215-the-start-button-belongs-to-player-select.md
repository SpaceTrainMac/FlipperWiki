---
rule: 0215
title: The start button belongs to player select, and a game in progress does not read it
source: FlipperVPX/docs/using-the-table.md § 4 — Playing it
as-of: 094e1fe
body: vpx
supersedes:
---
[using-the-table.md § 4 — Playing it](../../../FlipperVPX/docs/using-the-table.md#4--playing-it)

**The start button belongs to player select, and a game in progress does not read it.** Pressing
**1** or **S** as the last act of player select is what serves the first ball; after that every ball comes out
by itself, and nothing you can press during a game asks for one. **This paragraph said the opposite
earlier on 2026-09-05 and was wrong** — it had a saved ball waiting for a press, which is what the
engine did until that afternoon.
[gameplay.md §12](../../../FlipperArchitecture/docs/gameplay.md#12-the-ball-the-turn-and-the-game)
is the rule and now says the same.
