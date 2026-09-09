---
rule: 0063
title: One step per lit lamp, 200 ms apart
source: FlipperArchitecture/docs/gameplay.md § 10. The end of a ball: the count
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 10. The end of a ball: the count](../../../FlipperArchitecture/docs/gameplay.md#10-the-end-of-a-ball-the-count)

**One step per lit lamp, 200 ms apart.** Each step puts one lamp out and adds what that lamp stood
for to the turn score on the `MATCH` display, so the number climbs in visible pieces and the
playfield empties as it does.

| Lamp | Pays |
|---|---|
| `BON1_5K_BOT` … `BON9_5K_BOT` | 5 000 × the bottom multiplier |
| `SUPER_BON_10` / `_20` / `_30` | 50 000 × the bottom multiplier — each is ten bonuses |
| a hole-bonus rung, either side | 5 000 × that side's multiplier |
| `HOLE_BON_30K_L` / `_R`, armed | 30 000 × that side's multiplier |
