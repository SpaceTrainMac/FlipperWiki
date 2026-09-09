---
rule: 0284
title: HOUSE_BALL_SAVED — when it plays
source: FlipperEngine/docs/sound.md § 4. The catalogue - Effects, Ball and game lifecycle
as-of: 0e97ce3
body: game
supersedes:
---
[sound.md § 4. The catalogue - Effects, Ball and game lifecycle](../../../FlipperEngine/docs/sound.md#ball-and-game-lifecycle)

| Cue | The event | File | Shared with |
|---|---|---|---|
| `HOUSE_BALL_SAVED` | **A drain inside the 15-second protection window.** The ball is given back, nothing is counted and nothing is cleared, and the ejector serves it again as soon as the store has one - no press, since 2026-09-05. Fires **instead of** `BALL_LOST`, once per turn — the protection is spent the first time it saves a drain | `star-wars/R2D2-yeah.mp3` **fixture only** | `sfx.TOPLANES_SELECT_BONUS` |
