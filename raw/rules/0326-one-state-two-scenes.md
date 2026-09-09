---
rule: 0326
title: One state, two scenes
source: FlipperEngine/docs/states/intro.md § IntroMachine — inside the Intro state
as-of: 0e97ce3
body: game
supersedes:
---
[intro.md § IntroMachine — inside the Intro state](../../../FlipperEngine/docs/states/intro.md#intromachine--inside-the-intro-state)

**One state, two scenes.** `IntroMachine` itself is a dispatcher of about seventy lines; the
behaviour lives in two `IntroSceneMachine` subclasses that it runs in turn:
