---
rule: 0071
title: The two numbers together never change
source: FlipperArchitecture/docs/gameplay.md § 11. The end of a turn: the transfer
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 11. The end of a turn: the transfer](../../../FlipperArchitecture/docs/gameplay.md#11-the-end-of-a-turn-the-transfer)

**The two numbers together never change.** At every tick of the transfer, the turn score plus the
player's total is exactly what it was before it started — which is the whole correctness statement
about the mechanic, and the reason nothing can be lost or paid twice in the middle of it. A transfer
cut short by the cabinet being switched off finishes in one step, without the animation.
