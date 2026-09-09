---
rule: 0330
title: A display row is five steps of the animation, not one
source: FlipperEngine/docs/states/intro.md § IntroMachine — inside the Intro state
as-of: 0e97ce3
body: game
supersedes:
---
[intro.md § IntroMachine — inside the Intro state](../../../FlipperEngine/docs/states/intro.md#intromachine--inside-the-intro-state)

- **A display row is five steps of the animation, not one.** A digit has a height of its own, so the
  line crossing it is six shapes in order — `' '`, `_`, `u`, `o`, a 180°-rotated `A`, `8`
  (`src/actions/displayConst.hpp`) — and **nothing else on the glass moves while that happens**. Going
  down, a row drains to blank completely before the row below it starts.
