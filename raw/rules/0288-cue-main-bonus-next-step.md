---
rule: 0288
title: MAIN_BONUS_NEXT_STEP — when it plays
source: FlipperEngine/docs/sound.md § 4. The catalogue - Effects, The lower playfield
as-of: 0e97ce3
body: game
supersedes:
---
[sound.md § 4. The catalogue - Effects, The lower playfield](../../../FlipperEngine/docs/sound.md#the-lower-playfield)

| Cue | The event | File | Shared with |
|---|---|---|---|
| `MAIN_BONUS_NEXT_STEP` | **The bottom bonus ladder advances**, which is its README gloss and what the rules now make it: the four-target bank completing steps the count by exactly one ([gameplay.md §4](../../../FlipperArchitecture/docs/gameplay.md#4-the-advance-bonus-bank-and-the-combination)), and a `5000` inlane jumps it by five. **Once per advance, whatever its size** — not once per target hit, which pays 100 and moves nothing, and not five times for an inlane. **One cue for all thirty-nine rungs, carrying no index**, so nothing about the sound can say which rung it was | `star-wars/chewie.mp3` | `sfx.BUNKER_LEFT` |
