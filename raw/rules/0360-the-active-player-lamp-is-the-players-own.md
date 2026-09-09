---
rule: 0360
title: The active-player lamp is this class's
source: FlipperEngine/docs/states/game.md § GameMachine — The turn has two edges
as-of: 0e97ce3
body: game
supersedes:
---
[game.md § GameMachine — The turn has two edges](../../../FlipperEngine/docs/states/game.md#the-turn-has-two-edges)

**The active-player lamp is this class's.** `m_LED_ACTIVE_PLR` is picked in the constructor from
`player_id`, and the machine writes it twice a turn — lit at the beginning, out at the end. **A
player's own lamp is the one thing about a turn only that player's game knows**, and keeping it here
means a two-player game never touches lamps 169 or 171 at all, where a controller writing all four
would write one true and three false every turn.
