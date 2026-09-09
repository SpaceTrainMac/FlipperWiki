---
rule: 0278
title: The File column is the test fixture, and eleven rows are fixture only
source: FlipperEngine/docs/sound.md § 4. The catalogue
as-of: 0e97ce3
body: game
supersedes:
---
[sound.md § 4. The catalogue](../../../FlipperEngine/docs/sound.md#4-the-catalogue)

**The *File* column is [`tests/fixtures/sounds.json`](../../../FlipperEngine/tests/fixtures/sounds.json), and since
2026-09-04 that is no longer the same document as the shipped `rool` set.** The fixture has to name
a file for every cue — `theShippedMapCoversEveryCue` asserts it — and `rool` deliberately does not:
the eleven cues added that day are **absent from `rool/sounds.json` until a person finds an mp3 for
each**, because that set's value is that somebody with taste chose every file in it and synthesising
one would make it a fourth generated set wearing the first one's name
([the record §5](../../../FlipperSounds/docs/concepts/done/20260904-the-cues-the-rules-ask-for.md)).
So the eleven rows below are marked **fixture only**: what they name is what the *test* map plays,
and on a cabinet running `rool` they are silent.
