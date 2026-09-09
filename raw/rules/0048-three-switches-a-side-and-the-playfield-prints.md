---
rule: 0048
title: Three switches a side, and the playfield prints what each pays
source: FlipperArchitecture/docs/gameplay.md § 8. The side lanes, the sidebars and the bumpers
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 8. The side lanes, the sidebars and the bumpers](../../../FlipperArchitecture/docs/gameplay.md#8-the-side-lanes-the-sidebars-and-the-bumpers)

**Three switches a side, and the playfield prints what each pays.**

| Switch | Printed | Pays |
|---|---|---|
| `SIDELANE_LEFT` / `SIDELANE_RIGHT` | `500` | **500** |
| `SIDELANE_LEFT_5000` / `SIDELANE_RIGHT_5000` | `5000` | **5 000**, and five bonuses |
| `SIDELANE_LEFT_OUT` / `SIDELANE_RIGHT_OUT` | `SPECIAL` | **5 000** when `SPECIAL` is lit, and both `SPECIAL` lamps go out. Nothing when it is dark |
