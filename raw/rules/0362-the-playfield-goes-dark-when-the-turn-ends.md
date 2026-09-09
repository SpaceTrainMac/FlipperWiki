---
rule: 0362
title: The playfield goes dark when the turn ends
source: FlipperEngine/docs/states/game.md § GameMachine — The score on the glass, and the playfield between turns
as-of: 0e97ce3
body: game
supersedes:
---
[game.md § GameMachine — The score on the glass, and the playfield between turns](../../../FlipperEngine/docs/states/game.md#the-score-on-the-glass-and-the-playfield-between-turns)

- **The playfield goes dark when the turn ends.** `stopCurrentRound()` puts all 48 playfield lamps
  out after it has taken the games' own demands and cleared the continuous timers. **It is blunt on
  purpose**: several `src/games/` classes reset by *discarding* their pending demands rather than raising
  the opposite ones — `GameMAC` and `GameBumper` both call `clearActionDemands()` — so without the
  sweep a lamp lit on one ball would carry into the next player's. Clearing after the timers is what
  also settles a lamp left mid-blink, whose blink timer has just been thrown away.

The per-game fixes are still worth making where they are wrong; the sweep is what makes a forgotten
lamp cost nothing.
