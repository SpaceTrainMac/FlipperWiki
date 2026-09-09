---
rule: 0283
title: BALL_LOST — when it plays
source: FlipperEngine/docs/sound.md § 4. The catalogue - Effects, Ball and game lifecycle
as-of: 0e97ce3
body: game
supersedes:
---
[sound.md § 4. The catalogue - Effects, Ball and game lifecycle](../../../FlipperEngine/docs/sound.md#ball-and-game-lifecycle)

| Cue | The event | File | Shared with |
|---|---|---|---|
| `BALL_LOST` | **A drain that is not protected** — `BALLSENSOR_BALLCACHE` closes, `ballsInPlay` goes down, and the drain-protection window is shut or spent. A drain *inside* that window is a different event and gets `HOUSE_BALL_SAVED` ([gameplay.md §12](../../../FlipperArchitecture/docs/gameplay.md#12-the-ball-the-turn-and-the-game)). **Still not the end of the turn:** in multiball it fires with play continuing, and an extra ball in hand puts another one out. **Raised by the machine, and named after the games have read the same packet** (built 2026-09-08): a drain the saver covered is `HOUSE_BALL_SAVED`, a drain that was the lit `SPECIAL` outlane is `SPECIAL`, and everything else is this | `star-wars/swvader02.mp3` | — |
