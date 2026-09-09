---
rule: 0359
title: initNewRound is not the turn's edge and must not be confused with it
source: FlipperEngine/docs/states/game.md § GameMachine — The turn has two edges
as-of: 0e97ce3
body: game
supersedes:
---
[game.md § GameMachine — The turn has two edges](../../../FlipperEngine/docs/states/game.md#the-turn-has-two-edges)

| | `beginTurn()` — a ball is in play | `endTurn()` — no ball is in play |
|---|---|---|
| counters | `m_ballsOwed--`, `m_ballsPlayed++` | — |
| backglass | `GAME OVER` out; the active-player lamp lit; `AD1_DISPLAY_BALL_IN_PLAY` ← `m_ballsPlayed` | the active-player lamp out |
| playfield | `initNewRound()` — game state, `AR_NO_PADDLE_MODE` off, ball served | `stopCurrentRound()` — timers, playfield lamps; `AR_NO_PADDLE_MODE` **on** |

**`initNewRound()` is not the turn's edge and must not be confused with it.** It also runs mid-turn,
on an extra ball — which is exactly why the counters and the backglass are in `beginTurn()` and not
in it. An extra ball must not increment `BALL IN PLAY`; a regular turn must.
