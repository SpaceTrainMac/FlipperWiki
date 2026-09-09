---
rule: 0338
title: It is armed by the same number that arms the wait
source: FlipperEngine/docs/states/intro.md § IntroMachine — The two gestures
as-of: 0e97ce3
body: game
supersedes:
---
[intro.md § IntroMachine — The two gestures](../../../FlipperEngine/docs/states/intro.md#the-two-gestures)

**It is armed by the same number that arms the wait.** `radioGestureArmed()` is
`radioIdleSeconds > 0`, which `applySettings()` writes as zero for a cabinet with no station chosen
or with its sound switched off — so on a cabinet with no radio the gesture does nothing and the hint
never comes up. A second flag saying the same thing is a second flag that can disagree with the
first.
