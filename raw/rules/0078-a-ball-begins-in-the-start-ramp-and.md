---
rule: 0078
title: A ball begins in the start ramp, and the player fires it out by hand
source: FlipperArchitecture/docs/gameplay.md § 12. The ball, the turn and the game
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 12. The ball, the turn and the game](../../../FlipperArchitecture/docs/gameplay.md#12-the-ball-the-turn-and-the-game)

**A ball begins in the start ramp, and the player fires it out by hand.** The physical spring
plunger shoots it from there onto the playfield, and `OUTFIRE` at the end of the ramp is what sees
it go. There is no auto-launch on this cabinet: `FCA_1_BALL_OUT` fills the ramp and the player
empties it.
