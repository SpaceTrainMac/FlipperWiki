---
rule: 0339
title: Neither gesture can be mistaken for the other
source: FlipperEngine/docs/states/intro.md § IntroMachine — The two gestures
as-of: 0e97ce3
body: game
supersedes:
---
[intro.md § IntroMachine — The two gestures](../../../FlipperEngine/docs/states/intro.md#the-two-gestures)

**Neither gesture can be mistaken for the other**, and that takes two rules rather than one. Two
hands do not close two switches in the same millisecond, so a solo-flipper hold is counted only after
`SOLO_SETTLE_MS` of the other button being genuinely up — **and** any hold the other flipper was ever
seen down during is out for good until that button is released. The second rule is the one that is
easy to miss: without it, letting go of one hand halfway through a service gesture would start a
nine-second countdown to the radio.
