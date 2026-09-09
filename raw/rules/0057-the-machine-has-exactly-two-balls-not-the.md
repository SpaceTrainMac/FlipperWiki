---
rule: 0057
title: The machine has exactly two balls, not the flyer's three, and multiball cannot be fed a third
source: FlipperArchitecture/docs/gameplay.md § 9. The bunkers, and multiball
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 9. The bunkers, and multiball](../../../FlipperArchitecture/docs/gameplay.md#9-the-bunkers-and-multiball)

**The machine has exactly two balls, not the flyer's three, and multiball cannot be fed a third.**
`BALLSENSOR_BALLEJECTOR` reads no ball available for exactly as long as both balls are already on
the playfield, so a `BUNKER_LEFT` hit during an active multiball finds no ball to serve. The
multiball choreography above is skipped entirely for that hit — no hold, no wait for a second ball
that does not exist — and the bunker just spits the ball straight back out.
