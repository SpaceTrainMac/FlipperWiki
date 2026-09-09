---
rule: 0087
title: An extra ball is a number, and it is the two-digit field
source: FlipperArchitecture/docs/gameplay.md § 12. The ball, the turn and the game
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 12. The ball, the turn and the game](../../../FlipperArchitecture/docs/gameplay.md#12-the-ball-the-turn-and-the-game)

**An extra ball is a number, and it is the two-digit field.** Every award adds one to it, every
drain takes one away, and **the turn ends when a ball drains and that number is zero**. So the
player reads how much of their turn is left where a credit count used to be, and `BALL IN PLAY`
keeps meaning turns rather than balls.
