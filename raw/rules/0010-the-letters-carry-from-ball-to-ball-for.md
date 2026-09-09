---
rule: 0010
title: The letters carry from ball to ball for the whole game.
source: FlipperArchitecture/docs/gameplay.md § 3. M-A-C
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 3. M-A-C](../../../FlipperArchitecture/docs/gameplay.md#3-m-a-c)

**The letters carry from ball to ball for the whole game.** A player who had `M` and `C` lit when a
ball drained starts the next one with `M` and `C` lit, and a player who had all three lit starts the
next ball complete and paying — the completion path re-runs on the first cycle, re-blinking the
three lamps and re-lighting `SPECIAL`. **What does not carry is an open window**: `EXTRA_BALL_TOP`
is a lit award like any other, and [§12](../../../FlipperArchitecture/docs/gameplay.md#12-the-ball-the-turn-and-the-game) clears it with the rest
of the playfield when the ball ends.
