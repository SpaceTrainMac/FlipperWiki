---
rule: 0109
title: Every one of the 48, and what a lit one means
source: FlipperArchitecture/docs/gameplay.md § 13. What the machine shows
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 13. What the machine shows](../../../FlipperArchitecture/docs/gameplay.md#13-what-the-machine-shows)

**Every one of the 48, and what a lit one means.**

| Lamps | Lit means |
|---|---|
| `MAC_LEFT` / `_CENTER` / `_RIGHT` | that letter is spelled; all three blinking is M-A-C complete; `MAC_CENTER` flashing with `EXTRA_BALL_TOP` is `A`'s 20 s window |
| `ADV_BON_TOP` / `_C_TOP` / `_C_BOT` / `_BOT` | that advance-bonus target has been hit this bank; all four flash three times, then clear, on completion |
| `BON1_5K_BOT` … `BON9_5K_BOT` | the units of the bonus count |
| `SUPER_BON_10` / `_20` / `_30` | ten, twenty, thirty bonuses |
| `X2_BOT` / `X3_BOT` | the bonus count is doubled or tripled, for the rest of the game; `X3_BOT` lighting is the flyer's **Space Ship Bonus** |
| `BON1_TOP_L` … `BON5_TOP_L` | rungs of the **left** hole ladder; all five blink together with `HOLE_BON_30K_L` during that side's 30 s window |
| `BON1_5K_R` … `BON5_5K_R` | rungs of the **right** hole ladder; all five blink together with `HOLE_BON_30K_R` during that side's 30 s window |
| `BON_X2_TOP_L` / `BON_X3_TOP_L` | the left hole bonus is doubled or tripled, for the rest of the game |
| `BON_X2_5K_R` / `BON_X3_5K_R` | the right hole bonus is doubled or tripled, for the rest of the game |
| `HOLE_BON_30K_L` / `_R` | that side's 30 000 is armed; blinking with the five rungs means a 30 s redemption window is open, steady means the right captive ball armed it with no timer |
| `SPEC_5K_L` / `_R` | `SPECIAL` is lit — either outlane pays 5 000 |
| `EXTRA_BALL_TOP` | flashing with `MAC_CENTER`: an extra ball is waiting at the right captive ball for the 20 s `A`'s window runs. Nothing else lights it |
| `EXTRA_BALL_R` | an extra ball is waiting at the right captive ball, lit by the 2nd bank completion and staying lit until collected |
| `30K_TOP_L` / `_R` | the `M` lane and the `C` lane, while M-A-C is complete — the upper bank is M-A-C's display |
| `BUMPER_L` / `_R` / `_C` | flashed for 300 ms as that bumper is hit, together with a white flash on the cabinet's PWM backlight |
| `HOUSE_BALL` | the drain-protection window is open, next to the playfield's printed `EXTRA BALL` label |
| `X_BON` | the 40th or 50th total bank completion has opened its 20 s collection window |
