---
rule: 0095
title: The bottom-left display is one six-digit unit reading as three fields
source: FlipperArchitecture/docs/gameplay.md § 13. What the machine shows
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 13. What the machine shows](../../../FlipperArchitecture/docs/gameplay.md#13-what-the-machine-shows)

**The bottom-left display is one six-digit unit reading as three fields**, and two of its digits are
not fields at all:

| Digit | Address | Shows |
|---|---|---|
| 1 | 152 | `EXTRA PLAYS` — the winking eye |
| 2 | **153** | **nothing, ever** — painted over |
| 3 | 154 | `BALL IN PLAY` — turns left |
| 4 | **155** | **nothing, ever** — painted over |
| 5–6 | 156–157 | `CREDITS` — extra balls in hand |
