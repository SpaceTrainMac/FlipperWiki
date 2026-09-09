---
rule: 0058
title: It is also the left hole ladder's redemption point
source: FlipperArchitecture/docs/gameplay.md § 9. The bunkers, and multiball
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 9. The bunkers, and multiball](../../../FlipperArchitecture/docs/gameplay.md#9-the-bunkers-and-multiball)

**It is also the left hole ladder's redemption point**
([§6](../../../FlipperArchitecture/docs/gameplay.md#6-the-hole-bonuses-and-the-captive-balls)), and that part of the bunker's job does not care
whether a ball was cached. **A left marker armed with no window running — the right captive ball's
shortcut — is collected here too, at any time**, exactly as the right bunker collects a right one:
the two saucers are symmetric in everything the hole bonus asks of them. A hit here while the left
ladder's 30-second window is blinking pays the five rungs and the marker together, at the left
multiplier, and resets that ladder — on top of, not instead of, starting multiball when a ball is
available, and on top of the prompt eject when one is not. **When multiball does start, the ball
this hit put in the bunker leaves it exactly the way multiball always ejects one**: held until
`OUTFIRE` sees the freshly served second ball leave the ramp, then released 2.5 seconds after that.
