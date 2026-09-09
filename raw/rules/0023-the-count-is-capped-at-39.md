---
rule: 0023
title: The count is capped at 39
source: FlipperArchitecture/docs/gameplay.md § 5. The bonus count
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 5. The bonus count](../../../FlipperArchitecture/docs/gameplay.md#5-the-bonus-count)

**The count is capped at 39** and the lamps are the number written in two digits:

| Lamps | Stand for |
|---|---|
| `BON1_5K_BOT` … `BON9_5K_BOT`, the bottom ladder | the **units**, 0 to 9 |
| `SUPER_BON_10`, `_20`, `_30` | the **tens** — each lit as the count passes 10, 20 and 30 |

So a count of 25 shows five ladder lamps and the `10` and `20` Super Bonus lamps, and a count of 39
shows all nine and all three. **The arithmetic closes exactly**: `2 × 10 + 5` bonuses at 5 000 is
125 000, which is `25 × 5 000`.
