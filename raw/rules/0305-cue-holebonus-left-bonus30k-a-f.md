---
rule: 0305
title: HOLEBONUS_LEFT_BONUS30K_A to _F — when it plays
source: FlipperEngine/docs/sound.md § 4. The catalogue - Effects, The captive balls, hole bonus
as-of: 0e97ce3
body: game
supersedes:
---
[sound.md § 4. The catalogue - Effects, The captive balls, hole bonus](../../../FlipperEngine/docs/sound.md#the-captive-balls--hole-bonus)

| Cue | The event | File | Shared with |
|---|---|---|---|
| `HOLEBONUS_LEFT_BONUS30K_A` … `_F` | **The six items of a left redemption, counted out** — five rungs at 5 000 and the marker at 30 000, all at that side's multiplier, 55 000 before it and 165 000 at ×3. Six cues because six things are being paid at once, and a redemption that pays them to one sound says less than the playfield does. **Counted out 200 ms apart** (built 2026-09-08): the six ride one `ActionSequence`, at the pace the end-of-ball count walks a lamp, because six cues in one frame would play over each other | `swvader03` · `Laser_Blaster` · `900yearsold` · `blaster-firing` · `Laser_Blasts` · `Lightsaber_Turn_On`, all `star-wars/`, **`_B` … `_F` fixture only** | each letter with its `HOLEBONUS_RIGHT_BONUS30K_` twin; `_D` with `sfx.BUMPER`; `_F` with `sfx.LAUNCH_BALL` |
