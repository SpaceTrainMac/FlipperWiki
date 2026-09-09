---
rule: 0082
title: The ball comes back without a press, and that is a correction of 2026-09-05
source: FlipperArchitecture/docs/gameplay.md § 12. The ball, the turn and the game
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 12. The ball, the turn and the game](../../../FlipperArchitecture/docs/gameplay.md#12-the-ball-the-turn-and-the-game)

**The ball comes back without a press, and that is a correction of 2026-09-05.**
[D25](../../../FlipperArchitecture/docs/concepts/done/20260829-gameplay-mechanics.md) chose the opposite — *unlike a silent automatic
return*, the player was to re-launch the saved ball with `START` — and the machine's owner struck
that half of it: *as soon as we started the game (the transition from select player to playmachine),
we dont need to press the start button any more until we after we left the play machine*. **The
start button is player select's and the high score table's**, and the first ball of a game is served
by the press that ends player select rather than by one of its own. Everything else about D25 stands,
including the fifteen seconds and covering any drain.
