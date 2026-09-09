---
rule: 0290
title: BONUS_COUNT_STEP — when it plays
source: FlipperEngine/docs/sound.md § 4. The catalogue - Effects, The lower playfield
as-of: 0e97ce3
body: game
supersedes:
---
[sound.md § 4. The catalogue - Effects, The lower playfield](../../../FlipperEngine/docs/sound.md#the-lower-playfield)

| Cue | The event | File | Shared with |
|---|---|---|---|
| `BONUS_COUNT_STEP` | **One step of the end-of-ball count** — a lamp goes out, what it stood for is added to the turn score, 200 ms later the next one ([gameplay.md §10](../../../FlipperArchitecture/docs/gameplay.md#10-the-end-of-a-ball-the-count)). A quiet ball is 8 steps and everything-lit is 24, so **this is the one cue that must be short and must not stack**: 24 of anything at 200 ms is either a count or a mess, and which it is depends on the file rather than on the code | `star-wars/R2D2-do.mp3` **fixture only** | `sfx.NEXT_PLAYER` |
