---
rule: 0378
title: The number is read before the state hands over
source: FlipperEngine/docs/states/draw.md § The end-of-game draw
as-of: 0e97ce3
body: game
supersedes:
---
[draw.md § The end-of-game draw](../../../FlipperEngine/docs/states/draw.md#the-end-of-game-draw)

**The number is read before the state hands over**, which settles who holds `MATCH`:
`HighscoreMachine` writes the place being recorded to the same six digits for the whole of name entry
([20260819-highscore-entry.md §6](../../../FlipperEngine/docs/concepts/done/20260819-highscore-entry.md#6-what-is-on-the-glass)) and
runs shortly after this state on every game. So the draw dwells for three seconds — slept in slices,
so a shutdown is still noticed inside one — and then **blanks the display and the lamp itself**. One
consequence to watch on a real cabinet: the extra ball a winner earned is played with `MATCH` dark
rather than lit.
