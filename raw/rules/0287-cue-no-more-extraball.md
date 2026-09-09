---
rule: 0287
title: NO_MORE_EXTRABALL — when it plays
source: FlipperEngine/docs/sound.md § 4. The catalogue - Effects, Ball and game lifecycle
as-of: 0e97ce3
body: game
supersedes:
---
[sound.md § 4. The catalogue - Effects, Ball and game lifecycle](../../../FlipperEngine/docs/sound.md#ball-and-game-lifecycle)

| Cue | The event | File | Shared with |
|---|---|---|---|
| `NO_MORE_EXTRABALL` | **The two-digit field is at zero and a ball drains, so the turn is over.** Under [gameplay.md §12](../../../FlipperArchitecture/docs/gameplay.md#12-the-ball-the-turn-and-the-game) that field is *extra balls in hand* — every award adds one, every drain takes one, and the turn ends when a drain finds it empty. That is the one moment in a turn at which this sentence is true, and it is an announcement rather than a denial | `star-wars/Red_Alert.mp3` | `sfx.SPECIAL` |
