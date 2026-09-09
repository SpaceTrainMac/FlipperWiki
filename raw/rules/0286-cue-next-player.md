---
rule: 0286
title: NEXT_PLAYER — when it plays
source: FlipperEngine/docs/sound.md § 4. The catalogue - Effects, Ball and game lifecycle
as-of: 0e97ce3
body: game
supersedes:
---
[sound.md § 4. The catalogue - Effects, Ball and game lifecycle](../../../FlipperEngine/docs/sound.md#ball-and-game-lifecycle)

| Cue | The event | File | Shared with |
|---|---|---|---|
| `NEXT_PLAYER` | The turn passes — `PlayMachine` rotates to the next player's `GameMachine`, of which there is one per player. **To a different player** (built 2026-09-08): a one-player game never hears it, and the first turn of any game is nobody's turn passing | `star-wars/R2D2-do.mp3` | `sfx.BONUS_COUNT_STEP` |
