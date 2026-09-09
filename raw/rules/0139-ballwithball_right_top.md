---
rule: 0139
title: BALLWITHBALL_RIGHT_TOP — what closing it does
source: FlipperArchitecture/docs/gameplay.md § 2. Every switch, and what closing it does
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 2. Every switch, and what closing it does](../../../FlipperArchitecture/docs/gameplay.md#2-every-switch-and-what-closing-it-does)

| Switch | Pays | Advances | Collects |
|---|---|---|---|
| `BALLWITHBALL_RIGHT_TOP` | **500 000** if `X_BON` is flashing | lights **both** `HOLE BONUS 30000` lamps; lights `X2_BOT` or `X3_BOT` if `X_BON` is flashing | the right `EXTRA BALL` when it is lit (2nd bank completion); the **upper** `EXTRA BALL` inside `A`'s 20 s window |
