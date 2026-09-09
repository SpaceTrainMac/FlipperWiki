---
rule: 0002
title: A opens a 20-second window on the upper EXTRA BALL lamp
source: FlipperArchitecture/docs/gameplay.md § 3. M-A-C
as-of: cb52384
body: game
supersedes:
---
[gameplay.md § 3. M-A-C](../../../FlipperArchitecture/docs/gameplay.md#3-m-a-c)

**`A` opens a 20-second (configurable) window on the *upper* `EXTRA BALL` lamp.** `EXTRA_BALL_TOP`
and `MAC_CENTER` — the `A` lamp itself — flash together, which is the machine saying *hit the right
captive ball*. `BALLWITHBALL_RIGHT_TOP` inside the window awards the extra ball, with its own sound
cue and light effect; if the window closes first, nothing is awarded.
