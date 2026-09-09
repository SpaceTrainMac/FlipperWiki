---
rule: 0366
title: The coil is the operator's to switch off
source: FlipperEngine/docs/states/game.md § GameMachine — The high score announcement
as-of: 0e97ce3
body: game
supersedes:
---
[game.md § GameMachine — The high score announcement](../../../FlipperEngine/docs/states/game.md#the-high-score-announcement)

- **the coil is the operator's to switch off**, through a `knocker` key in settings.json. It gates
  the solenoid and not `FDLA_LED_HIGH_SCORE`: a quieter cabinet is not one that stops noticing.
