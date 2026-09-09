---
rule: 0347
title: The glass is dark on the way in, and that is the first thing this state does
source: FlipperEngine/docs/states/player-select.md § PlayerSelect — choosing the number of players
as-of: 0e97ce3
body: game
supersedes:
---
[player-select.md § PlayerSelect — choosing the number of players](../../../FlipperEngine/docs/states/player-select.md#playerselect--choosing-the-number-of-players)

**The glass is dark on the way in, and that is the first thing this state does.** Every one of the
six display groups is blanked and all sixteen backglass LEDs are written out, before anything is
drawn — because what is on the glass when this state is entered belongs to whoever was there before.
Attract mode leaves the high score walking across the score displays; a game that has just finished
leaves four totals, `GAME OVER` and a match number. None of it is true while somebody is deciding how
many are playing, and all of it used to stay there, because this machine wrote one digit and four
lamps and touched nothing else.
