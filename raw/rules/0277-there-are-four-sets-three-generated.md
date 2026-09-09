---
rule: 0277
title: There are four sets, and three of them are generated rather than collected
source: FlipperEngine/docs/sound.md § 4. The catalogue
as-of: 0e97ce3
body: game
supersedes:
---
[sound.md § 4. The catalogue](../../../FlipperEngine/docs/sound.md#4-the-catalogue)

**There are four sets**, and three of them are generated rather than collected. `8-bit` is composed:
35 files over the same cues, from scores that live with the set itself, in
`FlipperSounds/8-bit/generator/`, by that set's own `./generate.sh`. `space-opera` is the same idea
an orchestra wide — notation rendered through FluidSynth. `vocals` is spoken — two characters and a
narrator, generated from text scripts by its own TTS pipeline, and **it is the set the variant lists
exist for**: over a hundred effect scripts against the cues, twelve of them behind `BUMPER` alone.
All four map the same cues to the same events, so everything in the *event* column below is true of
all of them; only the *File* column belongs to one set. See
[concepts/done/20260822-eight-bit-sound-set.md](../../../FlipperEngine/docs/concepts/done/20260822-eight-bit-sound-set.md) for
why `8-bit` exists, and each set's own `README.md` for how to regenerate it. What each set turns the
cabinet into, with its icon, is [cabinet.md §3](../../../FlipperEngine/docs/cabinet.md#3-sound-sets).
