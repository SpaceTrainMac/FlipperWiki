---
rule: 0335
title: Two rates off one clock
source: FlipperEngine/docs/states/intro.md § IntroMachine — The high score scene
as-of: 0e97ce3
body: game
supersedes:
---
[intro.md § IntroMachine — The high score scene](../../../FlipperEngine/docs/states/intro.md#the-high-score-scene)

**Two rates off one clock.** The beat is 50 ms. The PWM backlight fade advances on every beat, which
is what a 64-step colour ramp wants; the lamp and display ladders advance on every *second* one, so
the line travelling up the cabinet is followable rather than a flicker. That is a divider
(`LADDER_BEATS_PER_STEP`) rather than a second deadline, because the two rates are meant to stay
locked together.
