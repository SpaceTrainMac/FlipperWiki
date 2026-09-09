---
title: The bonus ladder
type: thing
aliases: [the bonus ladder, the bottom ladder, BON1_5K_BOT, SUPER_BON_10, SUPER_BON_20, SUPER_BON_30, the Super Bonus lamps]
body: game
---
# The bonus ladder

**The bonus count is a row of lamps down the bottom of the playfield and a number nowhere.** It runs
0 to 39, it lasts one ball, and the only way to read it is to look at which lamps are lit ([0011](../../raw/rules/0011-ten-quantities-and-everything-below-is-one-of.md)).

**The lamps are the count written in two digits, and you read them like a number** ([0023](../../raw/rules/0023-the-count-is-capped-at-39.md)):

| Lamps | Stand for |
|---|---|
| `BON1_5K_BOT` … `BON9_5K_BOT`, the bottom ladder | the **units**, 0 to 9 |
| `SUPER_BON_10`, `_20`, `_30` | the **tens** — each lights as the count passes 10, 20 and 30 |

**So a count of 25 is five ladder lamps and the `10` and `20` Super Bonus lamps**, and 39 is all
nine and all three. The arithmetic closes exactly: 2 × 10 + 5 bonuses at 5 000 is 125 000, which is
25 × 5 000 ([0023](../../raw/rules/0023-the-count-is-capped-at-39.md)). **The count is capped at 39** ([0023](../../raw/rules/0023-the-count-is-capped-at-39.md)).

**The `X BONUS` printed down its side is this ladder, and it was never a multiplier.** The card's
*lights x BONUS* means one more lamp on the ladder — the first rung from empty, and the next one on
every completion after ([0017](../../raw/rules/0017-the-cards-x-bonus-is-the-ladder-and.md)).

**Every lamp on it is worth 5 000, paid when the ball ends and not before** ([0021](../../raw/rules/0021-one-number-from-0-to-39-worth-5.md)).

**Completing [the `ADVANCE BONUS` bank](../concepts/advance-bonus-bank.md) is what steps it.** A
single target hit does not ([0015](../../raw/rules/0015-each-target-on-its-first-hit-pays-100.md)); the fourth target completes the bank and the count advances one
step, lighting the next rung ([0016](../../raw/rules/0016-the-fourth-target-completes-the-bank.md)). **Either [`5000` inlane](inlanes-5000.md) steps it five at
once** ([0022](../../raw/rules/0022-what-advances-it.md)).

**Every ball starts it empty.** The bonus count is one of the things a drain clears, unlike the
multipliers and the M-A-C letters, which carry ([0013](../../raw/rules/0013-six-things-carry-from-one-ball-to-the.md)).

TBC — what lights a rung, and what the count pays, is not a rule here yet. What the machine
counts is [what the machine keeps track of](../concepts/what-the-machine-tracks.md).
