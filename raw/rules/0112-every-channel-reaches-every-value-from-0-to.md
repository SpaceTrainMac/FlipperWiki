---
rule: 0112
title: Every channel reaches every value from 0 to 15
source: FlipperArchitecture/docs/gameplay.md § 13. What the machine shows
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 13. What the machine shows](../../../FlipperArchitecture/docs/gameplay.md#13-what-the-machine-shows)

**Every channel reaches every value from 0 to 15.** Red covers 0–9 in the first decade, 2–11 in the
second, 4–13 in the third and 6–15 in the fourth, so all sixteen are reachable; green and blue cover
0–5, then 5–10 with `DOUBLE`, then 10–15 with `TRIPLE`. Neither wastes a step of the brightness the
cabinet has, and neither stops at 14.
