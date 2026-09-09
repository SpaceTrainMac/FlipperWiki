---
rule: 0294
title: SIDEBARS_BOTTOM — when it plays
source: FlipperEngine/docs/sound.md § 4. The catalogue - Effects, The lower playfield
as-of: 0e97ce3
body: game
supersedes:
---
[sound.md § 4. The catalogue - Effects, The lower playfield](../../../FlipperEngine/docs/sound.md#the-lower-playfield)

| Cue | The event | File | Shared with |
|---|---|---|---|
| `SIDEBARS_BOTTOM` | Either bottom sidebar — the two slingshots beside the flippers. They fire their own coils through the fast-action path and **score nothing** ([games.md §4.2](../../../FlipperEngine/docs/games.md#42-hardware-the-rules-use-but-the-code-never-touches)), so this is the one cue whose event is presentation and nothing else | `star-wars/blaster-firing.mp3` | `sfx.BUMPER`, both `NORMAL_HIT`s, both `BONUS30K_D`s |
