---
rule: 0088
title: What survives an extra ball is what survives any ball
source: FlipperArchitecture/docs/gameplay.md § 12. The ball, the turn and the game
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 12. The ball, the turn and the game](../../../FlipperArchitecture/docs/gameplay.md#12-the-ball-the-turn-and-the-game)

**What survives an extra ball is what survives any ball**: the three multipliers, the three M-A-C
letters, and the turn score.

| | Counted first | Playfield cleared | Turn score kept | `BALL IN PLAY` |
|---|---|---|---|---|
| **Drain protection** | no | no | yes | unchanged |
| **Extra ball** | yes | **yes** | yes | unchanged |
| **Multiball, one ball lost** | no | no | yes | unchanged |
| **The turn ending** | yes | yes | transferred, then zero | counts down |
