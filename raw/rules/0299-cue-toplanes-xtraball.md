---
rule: 0299
title: TOPLANES_XTRABALL — when it plays
source: FlipperEngine/docs/sound.md § 4. The catalogue - Effects, The upper playfield
as-of: 0e97ce3
body: game
supersedes:
---
[sound.md § 4. The catalogue - Effects, The upper playfield](../../../FlipperEngine/docs/sound.md#the-upper-playfield--the-m-a-c-lanes)

| Cue | The event | File | Shared with |
|---|---|---|---|
| `TOPLANES_XTRABALL` | **The upper extra ball, collected at the right captive ball.** The cue keeps its name and its *event moved*: `A` opens a 20 s window on `EXTRA_BALL_TOP` and the award is taken at `BALLWITHBALL_RIGHT_TOP` inside it, not at the lane ([gameplay.md §3](../../../FlipperArchitecture/docs/gameplay.md#3-m-a-c)). A window that closes uncollected pays nothing and raises nothing | `star-wars/force.mp3` | `sfx.SPACE_SHIP_BONUS` |
