---
rule: 0280
title: What each cue is for is written down here and nowhere else
source: FlipperEngine/docs/sound.md § 4. The catalogue
as-of: 0e97ce3
body: game
supersedes:
---
[sound.md § 4. The catalogue](../../../FlipperEngine/docs/sound.md#4-the-catalogue)

**What each cue is *for* is written down here and nowhere else, and as of 2026-09-04 all forty of
them are written down.** The *event* column is not a description of code: it is what the cue name
and the rules ([gameplay.md](../../../FlipperArchitecture/docs/gameplay.md)) say it is for, **and it is
the specification the callers were held to when they were written, on 2026-09-08** - one
`ActionSFX(...)` per row, in the game or the machine that owns the event, and every raise is pinned by
a test in `tests/testGames.cpp`, `tests/testHighscoreMachine.cpp` or `tests/testPlayMachine.cpp`.
Where a row left something open - which of two cues gives way, whether an interval is needed, how
six cues are counted out - the build decided it, and the row carries the decision with the date, so
that the column stays the specification and the code stays held to it. Five cues stood here as
**TBC** for want of a rule to attach them to; the rules exist now and
[the record §3](../../../FlipperSounds/docs/concepts/done/20260904-the-cues-the-rules-ask-for.md)
settled all five — [what settled them](../../../FlipperEngine/docs/sound.md#what-settled-the-five) is kept below the tables, along with
[the four events that still have no cue](../../../FlipperEngine/docs/sound.md#four-events-with-no-cue-and-why-that-is-not-eleven-more).
