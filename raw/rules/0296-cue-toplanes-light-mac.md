---
rule: 0296
title: TOPLANES_LIGHT_MAC — when it plays
source: FlipperEngine/docs/sound.md § 4. The catalogue - Effects, The upper playfield
as-of: 0e97ce3
body: game
supersedes:
---
[sound.md § 4. The catalogue - Effects, The upper playfield](../../../FlipperEngine/docs/sound.md#the-upper-playfield--the-m-a-c-lanes)

| Cue | The event | File | Shared with |
|---|---|---|---|
| `TOPLANES_LIGHT_MAC` | An `M`, `A` or `C` rollover **toggles** its letter while M-A-C is still being spelled — a dark lane lights, a lit lane goes out ([gameplay.md §3](../../../FlipperArchitecture/docs/gameplay.md#3-m-a-c)). **Not on the frame that completes the word** (built 2026-09-08): that frame is `TOPLANES_SUPERBONUS`'s and is no longer spelling | `star-wars/light-saber-on.mp3` | — |
