---
rule: 0084
title: It covers an outlane as readily as the middle
source: FlipperArchitecture/docs/gameplay.md § 12. The ball, the turn and the game
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 12. The ball, the turn and the game](../../../FlipperArchitecture/docs/gameplay.md#12-the-ball-the-turn-and-the-game)

**It covers an outlane as readily as the middle**, and that is a decision rather than a limitation.
The machine *can* tell them apart — an outlane closes `SIDELANE_LEFT_OUT` or `SIDELANE_RIGHT_OUT`
immediately before `BALLSENSOR_BALLCACHE`, and a drain with no such switch in front of it is a
centre drain — and the distinction is dropped regardless, to guarantee fun and avoid frustrating the
player.
