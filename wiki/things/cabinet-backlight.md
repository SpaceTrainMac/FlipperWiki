---
title: The cabinet backlight
type: thing
aliases: [the backlight, the cabinet backlight, FDLA_PWM_RED, FDLA_PWM_GREEN, FDLA_PWM_BLUE, the PWM backlight]
body: game
---
# The cabinet backlight

**A white flash means a bumper or a slingshot just fired.** The three channels are each 0–15; a hit
drives all three to 15 — full on every channel reads as white — for the same 300 ms the bumper's own
lamp is lit, and then the backlight goes back to whatever it was showing ([0053](../../raw/rules/0053-a-bumper-or-a-slingshot-hit-also-flashes.md)).

**Four flashes — two short, two long — is [a thunderstrike](../concepts/the-thunderstrike.md)**:
all three bumpers inside one second ([0054](../../raw/rules/0054-landing-all-three-bumpers-within-one-second-of.md)).

**The slingshots flash it too, on their own kick, and they still score nothing** ([0053](../../raw/rules/0053-a-bumper-or-a-slingshot-hit-also-flashes.md), [0051](../../raw/rules/0051-the-two-slingshots-kick-and-score-nothing.md)).

**At rest it is the two bonus ladders in colour, and the white flashes are a brief interruption of
that** ([0110](../../raw/rules/0110-not-a-playfield-lamp.md)). Each channel is independently 0–15:

| Channel | Tracks | Formula |
|---|---|---|
| **red** | [the bonus count](../concepts/the-bonus-count.md) | that ladder's units digit (0–9) **+ 2 for every Super Bonus lamp lit** |
| **green** | [the left hole bonus](../concepts/the-hole-bonus.md) | that side's rung count (0–5) **+ 5 for `DOUBLE`, + 5 more for `TRIPLE`** |
| **blue** | the right hole bonus | that side's rung count (0–5) **+ 5 for `DOUBLE`, + 5 more for `TRIPLE`** |

*(the table is rule 0110's, rendered for a player)*
