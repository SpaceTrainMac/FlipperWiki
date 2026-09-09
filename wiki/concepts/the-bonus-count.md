---
title: The bonus count
type: concept
aliases: [the bonus count, the bonus, BONUS COUNTS AT END OF BALL]
body: game
---
# The bonus count

**One number from 0 to 39, worth 5 000 each, and paid when the ball ends and not before** ([0021](../../raw/rules/0021-one-number-from-0-to-39-worth-5.md)).
The 1987 card says it plainly — *BONUS COUNTS AT END OF BALL* — and it is the mechanic that decides
what a good ball is worth ([0021](../../raw/rules/0021-one-number-from-0-to-39-worth-5.md)).

**A full count is 195 000** — 39 at 5 000 — before any multiplier ([0021](../../raw/rules/0021-one-number-from-0-to-39-worth-5.md)). You see it on
[the bonus ladder](../things/bonus-ladder.md), and nowhere as a number ([0027](../../raw/rules/0027-nothing-shows-the-count-as-a-number.md)).

**Where 39 comes from is the lamp table, not a designer's round number** ([0204](../../raw/rules/0204-up-to-39-bonuses-falls-out-of-the-lamp-table.md)):

| | Lamps | Worth |
|---|---|---|
| [the bottom ladder](../things/bonus-ladder.md) | `BON1_5K_BOT` … `BON9_5K_BOT` | **9** |
| [Super Bonus](../things/bonus-ladder.md) | `SUPER_BON_10` / `_20` / `_30` | **30** |
| | | **39** |

*(the table is machine.md §1.6's, rendered for a player ([0204](../../raw/rules/0204-up-to-39-bonuses-falls-out-of-the-lamp-table.md)))*

**So the flyer's *Up to 39 Bonuses* is a count of what the lamps can say**, and the cap is the
ladder's arithmetic rather than a rule laid on top of it ([0204](../../raw/rules/0204-up-to-39-bonuses-falls-out-of-the-lamp-table.md)).

**Two things advance it, and nothing else does** ([0022](../../raw/rules/0022-what-advances-it.md)):

| What you hit | Bonuses |
|---|---|
| [completing the four-target bank](advance-bonus-bank.md), all four lit | **+1** |
| either [`5000` inlane](../things/inlanes-5000.md) | **+5** |

**So an inlane is worth five bank completions to the count** — 25 000 at the end of the ball against
a completion's 5 000, and that is on top of the 5 000 the inlane pays at once ([0022](../../raw/rules/0022-what-advances-it.md)).

**It is capped at 39**, and [the ladder](../things/bonus-ladder.md) shows it as two digits — nine
unit lamps and three Super Bonus lamps for the tens ([0023](../../raw/rules/0023-the-count-is-capped-at-39.md)).

**Nothing about the count is paid as it climbs, and the shots that climb it are paid anyway.** The
100 an `ADVANCE BONUS` target pays is the switch's own award, whether or not that hit completes the
bank; the 5 000 an inlane pays is the same. What is deferred is the bonus, and only that ([0028](../../raw/rules/0028-nothing-about-the-count-is-paid-as-it.md)).

**At ×3 a full count is 585 000 a ball** ([0047](../../raw/rules/0047-what-survives-with-them-is-a-number-that.md)), and *1987* worked the same
arithmetic off the printing on the playfield ([0205](../../raw/rules/0205-with-bonus-x-5000-printed-on-the-playfield.md)):

| | Count | × 5 000 | `DOUBLE` | `TRIPLE` |
|---|---|--:|--:|--:|
| **maximum bonus** | 39 | 195 000 | 390 000 | **585 000** |

*(the table is machine.md §1.6's, rendered for a player ([0205](../../raw/rules/0205-with-bonus-x-5000-printed-on-the-playfield.md)). It is the same 585 000
[the multipliers](the-multipliers.md) reach, arrived at from the paint rather than from the code.)*

**The bottom `DOUBLE` and `TRIPLE` multiply it and nothing else** ([0038](../../raw/rules/0038-three-independent-pairs-of-double-triple-lamps-and.md)) — see
[the three multipliers](the-multipliers.md).

**Past the 39th the ladder stops moving, and the bank does not.** A completion still pays its flat
10 000 and still advances the combination while a stage is left, but the count goes no higher — so
the end-of-ball bonus never exceeds 195 000 before multipliers ([0025](../../raw/rules/0025-past-the-39th-bonus-the-ladder-stops-moving.md)).
