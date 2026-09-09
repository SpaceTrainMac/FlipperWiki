---
rule: 0019
title: Four awards are lit on a timer instead, and a flashing lamp is how the machine says so.
source: FlipperArchitecture/docs/gameplay.md § 4. The advance-bonus bank, and the combination
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 4. The advance-bonus bank, and the combination](../../../FlipperArchitecture/docs/gameplay.md#4-the-advance-bonus-bank-and-the-combination)

**Four awards are lit on a timer instead, and a flashing lamp is how the machine says so.** A window
that closes uncollected pays nothing at all:

| Windowed award | Runs for | Lamp |
|---|---|---|
| the upper `EXTRA BALL`, after `A` | 20 s | `EXTRA_BALL_TOP` with `MAC_CENTER` |
| the extra bonus, at the 40th and 50th completion | 20 s | `X_BON` |
| a hole-bonus redemption, either side | 30 s | that side's five rungs with its `HOLE BONUS 30000` |
| drain protection | 15 s | `HOUSE_BALL` |
