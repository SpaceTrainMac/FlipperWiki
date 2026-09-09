---
rule: 0328
title: The playfield is walked in rows, not in wiring order
source: FlipperEngine/docs/states/intro.md § IntroMachine — inside the Intro state
as-of: 0e97ce3
body: game
supersedes:
---
[intro.md § IntroMachine — inside the Intro state](../../../FlipperEngine/docs/states/intro.md#intromachine--inside-the-intro-state)

- **The playfield is walked in rows, not in wiring order.** Lamps are grouped by their `y` in
  `web/playfield.json` at a tolerance of 12 units, and every row fires as one `ActionGroup` — so
  `BON_X3_TOP_L` (192), `X_BON` (197) and `BON_X2_5K_R` (211), which sit within ten units of each
  other, light on the same step. The sequence this replaced climbed the right-hand bank to y=50 and
  then dropped back to y=86 to start again.
