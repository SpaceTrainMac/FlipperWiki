---
rule: 0289
title: MAIN_BONUS_ONE_LIGHT — when it plays
source: FlipperEngine/docs/sound.md § 4. The catalogue - Effects, The lower playfield
as-of: 0e97ce3
body: game
supersedes:
---
[sound.md § 4. The catalogue - Effects, The lower playfield](../../../FlipperEngine/docs/sound.md#the-lower-playfield)

| Cue | The event | File | Shared with |
|---|---|---|---|
| `MAIN_BONUS_ONE_LIGHT` | **The ladder reaching 39 and stopping.** Nine ladder lamps and all three `SUPER_BON`s lit is the count's cap ([gameplay.md §5](../../../FlipperArchitecture/docs/gameplay.md#5-the-bonus-count)); past it a bank completion still pays its flat 10 000 and the ladder does not move. The ladder has exactly one terminal state and this is it. **Raised instead of `MAIN_BONUS_NEXT_STEP` on that advance, not beside it** (built 2026-09-08): the terminal advance is one event, and an advance at the cap moves nothing and says nothing | `star-wars/set-for-stun.mp3` | — |
