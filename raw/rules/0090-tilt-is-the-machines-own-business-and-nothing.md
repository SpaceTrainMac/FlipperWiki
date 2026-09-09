---
rule: 0090
title: Tilt is the machine's own business, and nothing here can see one
source: FlipperArchitecture/docs/gameplay.md § 12. The ball, the turn and the game
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 12. The ball, the turn and the game](../../../FlipperArchitecture/docs/gameplay.md#12-the-ball-the-turn-and-the-game)

**Tilt is the machine's own business, and nothing here can see one.** The cabinet kills its own
outputs until the balls have drained and never tells the host, which sees an ordinary drain and
counts the bonus for it. **So a tilt does not void the ball's bonus** — none of the 32 matrix inputs
is a tilt bob ([hardware.md, *no tilt switch*](../../../FlipperArchitecture/docs/hardware.md#no-tilt-switch)), so voiding it is not
one of the behaviours available. What the player loses to a tilt is every output the cabinet has
just switched off, which is punishment enough.
