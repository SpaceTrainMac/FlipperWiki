---
rule: 0212
title: D4 — The three sidelane switches are the three printed values
source: FlipperArchitecture/docs/machine.md § 1.7 Decided where the sources are silent
as-of: 0804fe1
body: 1987
supersedes:
---
[machine.md § 1.7 Decided where the sources are silent](../../../FlipperArchitecture/docs/machine.md#17-decided-where-the-sources-are-silent)

| # | Decided | From |
|---|---|---|
| **D4** | **The three sidelane switches are the three printed values**: `_OUT` is the outlane and pays `SPECIAL` when lit, `_5000` is the inlane and pays 5 000, and the plain `SIDELANE_LEFT` / `_RIGHT` pay 500 | [§1.4](../../../FlipperArchitecture/docs/machine.md#14-playfield-geography): the outlanes and inlanes are printed `SPECIAL`, `5000` and `500`, and there are exactly three switches a side. `SIDELANE_*_5000` already pays 5 000 in `GameSuperBonus`, which fixes one of the three and leaves the other two in the only order that fits |
