---
rule: 0069
title: When the turn is over, the number on the `MATCH` display walks across to the player's own
source: FlipperArchitecture/docs/gameplay.md § 11. The end of a turn: the transfer
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 11. The end of a turn: the transfer](../../../FlipperArchitecture/docs/gameplay.md#11-the-end-of-a-turn-the-transfer)

**When the turn is over, the number on the `MATCH` display walks across to the player's own.** The
turn score counts down to zero and the player's total counts up by the same amount, in **20 ticks of
100 ms — 2.0 seconds, whatever the number is**.
