---
rule: 0422
title: The backlight is three waves rather than one
source: FlipperEngine/docs/states/credits.md § CreditsMachine — The light show
as-of: 0e97ce3
body: game
supersedes:
---
[credits.md § CreditsMachine — The light show](../../../FlipperEngine/docs/states/credits.md#the-light-show)

**The backlight is three waves rather than one.** Red gets wavelength 1 (4 s), green 2, blue 4, each
mapped from `sin` onto the channel's 0–15. Three periods in that ratio share a common period of four,
so the colour repeats every 16 seconds and passes through a different mix on the way each time; one
wave on all three channels would have been a backglass pulsing white, which is a duller thing
entirely. The brightness is a function of *elapsed wall time*, not of a tick count, for the same
reason the duration is — how fast the machine ticks is a display concern, and a faster tick must not
make the colours cycle faster. Only channels whose brightness has actually changed are written, which
on a 20 Hz cycle against a 4-second wave is most cycles saying nothing.
