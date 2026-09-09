---
rule: 0018
title: The lit awards wait to be collected, which is the grammar the 1987 card uses throughout.
source: FlipperArchitecture/docs/gameplay.md § 4. The advance-bonus bank, and the combination
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 4. The advance-bonus bank, and the combination](../../../FlipperArchitecture/docs/gameplay.md#4-the-advance-bonus-bank-and-the-combination)

**The lit awards wait to be collected, which is the grammar the 1987 card uses throughout.**
*Lights* an award and *gives* an award are two different verbs on that card: a lamp that is lit
stays lit until the switch that collects it closes, or until the ball ends.

| Award | Lit by | Collected at |
|---|---|---|
| `SPECIAL`, both lamps | M-A-C completing, or the 3rd bank completion | either outlane — `SIDELANE_LEFT_OUT` or `SIDELANE_RIGHT_OUT` |
| upper `EXTRA BALL` | `A`, with M-A-C complete — a 20 s window | `BALLWITHBALL_RIGHT_TOP`, the right captive ball |
| right `EXTRA BALL` | the 2nd bank completion, and nothing else — it stays lit until collected | `BALLWITHBALL_RIGHT_TOP`, the right captive ball |
| `HOLE BONUS 30000`, per side | that side's ladder reaching its 5th hit, or the right captive ball | that side's own bunker, or the end of the ball |
