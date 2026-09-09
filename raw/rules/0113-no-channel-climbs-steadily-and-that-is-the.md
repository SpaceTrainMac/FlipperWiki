---
rule: 0113
title: No channel climbs steadily, and that is the point rather than a defect
source: FlipperArchitecture/docs/gameplay.md § 13. What the machine shows
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 13. What the machine shows](../../../FlipperArchitecture/docs/gameplay.md#13-what-the-machine-shows)

**No channel climbs steadily, and that is the point rather than a defect.** Red reads the units
digit, so it *falls* every time the count crosses a ten:

| Bonus count | 9 | 10 | 19 | 20 | 29 | 30 | 39 |
|---|---|---|---|---|---|---|---|
| `FDLA_PWM_RED` | 9 | 2 | 11 | 4 | 13 | 6 | 15 |
