---
rule: 0437
title: There are five sets, and four of them are generated rather than collected
source: FlipperEngine/docs/sound.md § 4. The catalogue
as-of: be47236
body: game
supersedes: 0277
---
[sound.md § 4. The catalogue](../../../FlipperEngine/docs/sound.md#4-the-catalogue)

**There are five sets**, and four of them are generated rather than collected. `8-bit` is composed:
35 files over the same cues, from scores that live with the set itself, in
`FlipperSounds/8-bit/generator/`, by that set's own `./generate.sh`. `space-opera` is the same idea
an orchestra wide — notation rendered through FluidSynth. `vocals` is spoken — two characters and a
narrator, generated from text scripts by its own TTS pipeline, and **it is the set the variant lists
exist for**: over a hundred effect scripts against the cues, twelve of them behind `BUMPER` alone.
`rock-opera`, added 2026-09-17, is a band — guitar, organ, bass and a kit through FluidSynth — with
**a voice that sings rather than speaks**, its lyrics rendered through a DiffSinger voicebank, and
**it is the first set a fresh clone cannot build unattended**, because that bank is somebody else's
property and a person has to accept its terms
([the record](../../../FlipperSounds/docs/concepts/done/20260917-rock-opera-sound-set.md)).
All five map the same cues to the same events, so everything in the *event* column below is true of
all of them; only the *File* column belongs to one set. See
[concepts/done/20260822-eight-bit-sound-set.md](../../../FlipperEngine/docs/concepts/done/20260822-eight-bit-sound-set.md) for
why `8-bit` exists, and each set's own `README.md` for how to regenerate it. What each set turns the
cabinet into, with its icon, is [cabinet.md §3](../../../FlipperEngine/docs/cabinet.md#3-sound-sets).
