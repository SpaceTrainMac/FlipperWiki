---
rule: 0099
title: The fifth display divides by ten too, and has no lamp to say so
source: FlipperArchitecture/docs/gameplay.md § 13. What the machine shows
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 13. What the machine shows](../../../FlipperArchitecture/docs/gameplay.md#13-what-the-machine-shows)

**The fifth display divides by ten too, and has no lamp to say so.** A turn is a ball plus every
extra ball it earns, and [§10](../../../FlipperArchitecture/docs/gameplay.md#10-the-end-of-a-ball-the-count)'s ceiling is 915 000 for one ball —
so a turn passes six digits as soon as one extra ball goes well.
[hardware.md §3](../../../FlipperArchitecture/docs/hardware.md#3-display-indicator-leds) has four `×10` indicators, one per player,
and none for `MATCH`. **So the turn score is not capped at 999 999 — the display is**, and past that
it silently shows a tenth of the number.
