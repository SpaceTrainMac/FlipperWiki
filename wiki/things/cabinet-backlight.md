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

**Each formula tops out at exactly 15, the channel's own maximum, at that ladder's own maximum.** A
bonus count of 39 is nine units plus three Super Bonus lamps — 9 + 2 × 3 = 15; five rungs at
`TRIPLE` is 5 + 5 + 5 = 15 ([0111](../../raw/rules/0111-each-formula-tops-out-at-exactly-15-the.md)).

**Every channel reaches every value from 0 to 15.** Red covers 0–9 in the first decade, 2–11 in the
second, 4–13 in the third and 6–15 in the fourth; green and blue cover 0–5, then 5–10 with `DOUBLE`,
then 10–15 with `TRIPLE`. Neither wastes a step of the brightness the cabinet has ([0112](../../raw/rules/0112-every-channel-reaches-every-value-from-0-to.md)).

**No channel climbs steadily, and that is the point rather than a defect.** Red reads the units
digit, so it *falls* every time the count crosses a ten ([0113](../../raw/rules/0113-no-channel-climbs-steadily-and-that-is-the.md)):

| Bonus count | 9 | 10 | 19 | 20 | 29 | 30 | 39 |
|---|--:|--:|--:|--:|--:|--:|--:|
| red | 9 | 2 | 11 | 4 | 13 | 6 | 15 |

*(the table is rule 0113's, rendered for a player)*

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
