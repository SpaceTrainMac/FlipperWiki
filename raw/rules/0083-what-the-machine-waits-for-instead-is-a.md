---
rule: 0083
title: What the machine waits for instead is a ball
source: FlipperArchitecture/docs/gameplay.md § 12. The ball, the turn and the game
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 12. The ball, the turn and the game](../../../FlipperArchitecture/docs/gameplay.md#12-the-ball-the-turn-and-the-game)

**What the machine waits for instead is a ball**, and the distinction is not a detail: the drained
ball needs the length of the trough to roll back under the ejector, so the serve is triggered by
`BALLSENSOR_BALLEJECTOR` reading *available to serve* and not by the drain that asked for it. A coil
fired at the drain kicks an empty pocket and leaves the ball in the store, which is what this rule
looked like when it was found.
