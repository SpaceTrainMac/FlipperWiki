---
rule: 0312
title: SPACE_SHIP_BONUS — when it plays
source: FlipperEngine/docs/sound.md § 4. The catalogue - Effects, The two the flyer names
as-of: 0e97ce3
body: game
supersedes:
---
[sound.md § 4. The catalogue - Effects, The two the flyer names](../../../FlipperEngine/docs/sound.md#the-two-the-flyer-names-and-the-one-that-pays-most)

| Cue | The event | File | Shared with |
|---|---|---|---|
| `SPACE_SHIP_BONUS` | **`X3_BOT` lighting** — the 50th bank completion, collected. A *space-engine warp*. **Announced once, at the moment the lamp lights, and never again**: `X3_BOT` stays lit for the rest of the game, so a rule that fired while the condition *held* would play the warp on every ball from then on | `star-wars/force.mp3` **fixture only** | `sfx.TOPLANES_XTRABALL` |
