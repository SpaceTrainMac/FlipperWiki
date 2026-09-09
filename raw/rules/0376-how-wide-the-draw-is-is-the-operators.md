---
rule: 0376
title: How wide the draw is, is the operator's
source: FlipperEngine/docs/states/draw.md § The end-of-game draw
as-of: 0e97ce3
body: game
supersedes:
---
[draw.md § The end-of-game draw](../../../FlipperEngine/docs/states/draw.md#the-end-of-game-draw)

**How wide the draw is, is the operator's**, and it is the `matchDigits` key in settings.json — 1 to
6, default 2. One digit is a draw in ten and two is the classic draw in a hundred. It is a width
rather than a probability because the number has to fit the display it is read from, and because
"the last two digits of your score" is the rule a player already knows.
