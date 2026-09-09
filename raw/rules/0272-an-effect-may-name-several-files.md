---
rule: 0272
title: An effect may name several files instead of one
source: FlipperEngine/docs/cabinet.md § 3. Sound sets - sounds.json, which file each cue plays
as-of: 0e97ce3
body: cabinet
supersedes:
---
[cabinet.md § 3. Sound sets - sounds.json, which file each cue plays](../../../FlipperEngine/docs/cabinet.md#soundsjson--which-file-each-cue-plays)

**An effect may name several files instead of one**, and then the cabinet picks between them each
time the cue fires — which is how a bumper stops sounding like the same bumper three hundred times an
evening:

```json
"sfx": { "BUMPER": ["sfx/bumper-1.mp3", "sfx/bumper-2.mp3", "sfx/bumper-3.mp3"] }
```

| | |
|---|---|
| **How it picks** | `sfxMode` in [§1](../../../FlipperEngine/docs/cabinet.md#1-the-settings-file), `SFX MODE` in the menu: `RANDOM` deals a shuffled deck and reshuffles when it runs out, `LOOP` walks them in the order written here. One switch for every multi-file cue in the set, and in force at once |
| **Where it is allowed** | `sfx` only. A list under `music` **stops the cabinet** with `E 101`: a music cue is one piece, and somebody who wrote variants for a cue that can only ever play one of them has to be told rather than warned at. A list *inside* `songs` is ignored with a warning instead — the playlist is already a list, and a track's position in it is how the jukebox addresses it |
| **How many** | as many as you like, and a list of one behaves exactly like a plain path |
| **Hearing them** | `SOUND TEST` names the variant it is playing and steps to the next one each time you come back to the cue ([states/hardware-tests.md](../../../FlipperEngine/docs/states/hardware-tests.md)) |
