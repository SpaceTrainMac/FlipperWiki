---
rule: 0297
title: TOPLANES_SELECT_BONUS — when it plays
source: FlipperEngine/docs/sound.md § 4. The catalogue - Effects, The upper playfield
as-of: 0e97ce3
body: game
supersedes:
---
[sound.md § 4. The catalogue - Effects, The upper playfield](../../../FlipperEngine/docs/sound.md#the-upper-playfield--the-m-a-c-lanes)

| Cue | The event | File | Shared with |
|---|---|---|---|
| `TOPLANES_SELECT_BONUS` | **The flipper buttons rotating the three letters** — the lane change, and the only *selection* the top lanes offer. **It needs no minimum interval, and this row asked for one** (built 2026-09-08): the concern was a held button rotating the letters once a game cycle, and a held button does no such thing — `isSensorTriggeredHigh()` is a rising flank, so a press is one rotation whatever it is held for, and the cue follows the rotation; a test pins that the same matrix arriving again rotates nothing. What a player can do is tap fast, and a tap that rotated the letters is a selection they made | `star-wars/R2D2-yeah.mp3` | `sfx.HOUSE_BALL_SAVED` |
