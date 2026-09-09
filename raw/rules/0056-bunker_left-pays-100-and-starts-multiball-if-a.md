---
rule: 0056
title: `BUNKER_LEFT` pays 100
source: FlipperArchitecture/docs/gameplay.md § 9. The bunkers, and multiball
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 9. The bunkers, and multiball](../../../FlipperArchitecture/docs/gameplay.md#9-the-bunkers-and-multiball)

`BUNKER_LEFT` pays **100**, and starts multiball **if a ball is cached and ready** —
`BALLSENSOR_BALLCACHE` confirms one is staged in the ball-loading area
([§12](../../../FlipperArchitecture/docs/gameplay.md#12-the-ball-the-turn-and-the-game)). When it starts, a second ball is served into the start
ramp from that same store: the bunker holds the first ball while the second is on its way, and
releases it **2.5 seconds after `OUTFIRE` sees that second ball leave the ramp**, so both are on the
playfield together. The second ball waits for the player's plunger like any other — this cabinet has
no auto-launch — so the hold lasts as long as the player takes over it, and the 2.5 seconds is
measured from the plunge and not from the serve.
