---
rule: 0012
title: The score moves only between turns, and that is the single most visible mechanic on the machine.
source: FlipperArchitecture/docs/gameplay.md § 1. What the machine keeps track of
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 1. What the machine keeps track of](../../../FlipperArchitecture/docs/gameplay.md#1-what-the-machine-keeps-track-of)

**The score moves only between turns, and that is the single most visible mechanic on the machine.**
Everything a player earns during a ball goes into the *turn score* on the `MATCH` display; their own
display holds the total they had when the turn began and does not move until the ball is over.
[§10](../../../FlipperArchitecture/docs/gameplay.md#10-the-end-of-a-ball-the-count) and [§11](../../../FlipperArchitecture/docs/gameplay.md#11-the-end-of-a-turn-the-transfer) are where the
two numbers meet.
