---
rule: 0336
title: There is no service button on this cabinet
source: FlipperEngine/docs/states/intro.md § IntroMachine — The two gestures
as-of: 0e97ce3
body: game
supersedes:
---
[intro.md § IntroMachine — The two gestures](../../../FlipperEngine/docs/states/intro.md#the-two-gestures)

**There is no service button on this cabinet** — all 32 matrix inputs are playfield switches plus the
three buttons ([hardware.md §1](../../../FlipperArchitecture/docs/hardware.md#1-switch-matrix)) — so the two things attract mode can
be asked for that are not a game are gestures on the flippers:

| | | |
|---|---|---|
| both flippers, held 9 s | `Setup` | `SETUP_GESTURE_MS`, with `TEASE_HEADLINE` and `TEASE_QUOTE` up at 3 s |
| the right flipper **alone**, held 9 s | `Radio` | `RADIO_GESTURE_MS`, with `RADIO_TEASE_HEADLINE` and `RADIO_TEASE_QUOTE` up at 3 s |
