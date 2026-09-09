---
rule: 0060
title: `BUNKER_RIGHT` is the card's hole for the right side
source: FlipperArchitecture/docs/gameplay.md § 9. The bunkers, and multiball
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 9. The bunkers, and multiball](../../../FlipperArchitecture/docs/gameplay.md#9-the-bunkers-and-multiball)

**`BUNKER_RIGHT` is the card's *hole* for the right side, and up to three things happen when a ball
lands in it:**

1. It pays **100**.
2. If either hole ladder is past rung 2, it awards an **extra ball** — once per ball.
3. If the right ladder's 30-second window is blinking, it redeems the five rungs and the marker
   together, at the right multiplier, and resets that ladder. A right marker armed with no window
   running — the right captive ball's shortcut — is collected here too, at any time.

It then kicks the ball back out after five seconds. The collection is two steps at most — the extra
ball and one redemption or marker — and fits inside that hold with room to spare.
