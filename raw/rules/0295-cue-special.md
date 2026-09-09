---
rule: 0295
title: SPECIAL — when it plays
source: FlipperEngine/docs/sound.md § 4. The catalogue - Effects, The lower playfield
as-of: 0e97ce3
body: game
supersedes:
---
[sound.md § 4. The catalogue - Effects, The lower playfield](../../../FlipperEngine/docs/sound.md#the-lower-playfield)

| Cue | The event | File | Shared with |
|---|---|---|---|
| `SPECIAL` | **Either outlane with `SPECIAL` lit** — 5 000, and both `SPECIAL` lamps go out ([gameplay.md §8](../../../FlipperArchitecture/docs/gameplay.md#8-the-side-lanes-the-sidebars-and-the-bumpers)). **It is the shot that pays and drains at once**, so `BALL_LOST` follows it immediately and one of the two has to give way — **and `BALL_LOST` does** (built 2026-09-08): the payout is the news, the lane leaves a flag in the shared playfield state, and the machine's drain reads it, clears it and stays quiet — unless drain protection is open, in which case the ball comes back and `HOUSE_BALL_SAVED` follows instead. `SPECIAL` is lit by M-A-C completing or by the 3rd bank completion, and a dark outlane raises nothing | `star-wars/Red_Alert.mp3` **fixture only** | `sfx.NO_MORE_EXTRABALL` |
