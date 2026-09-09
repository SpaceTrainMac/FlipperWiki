---
rule: 0400
title: The timeout commits rather than discards
source: FlipperEngine/docs/states/highscore.md § HighscoreMachine — How an entry ends
as-of: 0e97ce3
body: game
supersedes:
---
[highscore.md § HighscoreMachine — How an entry ends](../../../FlipperEngine/docs/states/highscore.md#how-an-entry-ends)

**The timeout commits rather than discards**, which is what makes it defensible where the 2026-08-05
sketch refused one: the objection was that a timeout could only take away a place already earned, and
this one does not. What it buys is that the cabinet is never stranded out of attract mode with half a
name standing on the glass. Ten minutes by default and a `nameEntrySeconds` key, because the timeout
is not there to hurry anybody: a place has been won, six characters is a lot to spell, and being
rushed off the glass mid-name is worse than a cabinet that takes a while to notice an empty room.
