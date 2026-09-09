---
rule: 0089
title: Multiball ends nothing
source: FlipperArchitecture/docs/gameplay.md § 12. The ball, the turn and the game
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 12. The ball, the turn and the game](../../../FlipperArchitecture/docs/gameplay.md#12-the-ball-the-turn-and-the-game)

**Multiball ends nothing.** A turn is over when nothing is owed and `BALLSENSOR_BALLCACHE` closes
and stays closed, so a drain while another ball is on the playfield — which pulses the contact and
releases it — changes nothing at all.
