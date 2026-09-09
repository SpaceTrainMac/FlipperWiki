---
title: The end of a ball
type: moment
aliases: [the end of a ball, when the ball ends, a drain]
body: game
---
# The end of a ball

**Every ball that ends is counted out lamp by lamp, and the machine is silent while it happens**
([0062](../../raw/rules/0062-every-ball-that-ends-is-counted-out-lamp.md)). This is what the 1987 card's *BONUS COUNTS AT END OF BALL* looks like from in front of the
glass ([0062](../../raw/rules/0062-every-ball-that-ends-is-counted-out-lamp.md)).

**One step per lit lamp, 200 ms apart.** Each step puts one lamp out and adds what it stood for to
the turn score on [the `MATCH` display](../things/match-display.md), so the number climbs in visible
pieces as the playfield empties ([0063](../../raw/rules/0063-one-step-per-lit-lamp-200-ms-apart.md)):

| Lamp | Pays |
|---|---|
| a bonus-ladder lamp | 5 000 × the bottom multiplier |
| a Super Bonus lamp, `10` / `20` / `30` | 50 000 × the bottom multiplier — each is ten bonuses |
| a hole-bonus rung, either side | 5 000 × that side's multiplier |
| an armed `HOLE BONUS 30000` | 30 000 × that side's multiplier |

*(the table is rule 0063's, rendered for a player)*

**How long it takes, at 200 ms a step** ([0066](../../raw/rules/0066-the-arithmetic-at-200-ms-a-step.md)):

| The ball | Steps | Time | Paid |
|---|---|--:|--:|
| a quiet one — five bonuses, one hole ladder at rung 3 | 8 | 1.6 s | 40 000 |
| a good one — 25 bonuses at ×2, one side at five rungs and armed | 13 | 2.6 s | 305 000 |
| everything lit — 39 bonuses at ×3, both sides full and armed, both at ×3 | 24 | 4.8 s | **915 000** |

*(the table is rule 0066's, rendered for a player)*

**Nothing scores while the count runs.** The playfield is empty by definition — the ball that
earned all of it is in the trough — but the machine still holds every other award, so a number being
counted out cannot be added to behind the walk ([0065](../../raw/rules/0065-nothing-scores-while-the-count-runs.md)).

**The two hole bonuses are counted first and the bonus ladder last**, which is the order the 1987
card lists them in. The multiplier lamps take no step and stay lit ([0064](../../raw/rules/0064-the-two-hole-bonuses-are-counted-first-and.md)).

**When a ball ends, the playfield's lit awards are cleared and the M-A-C letters are not.** The
upper `EXTRA BALL` window goes with the rest of the playfield; `M`, `A` and `C` carry to the next
ball, and three lit letters start it complete and paying ([0010](../../raw/rules/0010-the-letters-carry-from-ball-to-ball-for.md)).

**The multipliers are not spent by the count they multiply** — they stay lit into the next ball
([0042](../../raw/rules/0042-all-three-survive-the-ball-and-the-game.md)).

**Six things survive a ball and everything else starts again**: the three multipliers, how many
times you have completed the bank, the two redemption counts, the M-A-C letters, the extra balls you
have won, and the turn score. The next ball begins with the bonus count at zero, both hole ladders
empty, no marker armed and no award lit ([0013](../../raw/rules/0013-six-things-carry-from-one-ball-to-the.md)).

**It is when [the bonus count](../concepts/the-bonus-count.md) is paid** — 5 000 a bonus, up to 39
of them, and not a point of it before ([0021](../../raw/rules/0021-one-number-from-0-to-39-worth-5.md)).

**It pays whatever a hole ladder has standing** — 5 000 a rung and 30 000 a marker, at that side's
multiplier ([0034](../../raw/rules/0034-nothing-on-a-hole-ladder-pays-before-it.md)). **It banks a hole-bonus side that was still blinking.** A drain is not the same event as a window
expiring: whatever is lit at that instant is counted, timer or no timer ([0033](../../raw/rules/0033-letting-the-window-close-forfeits-the-attempt-outright.md)).

TBC — what else the end of a ball pays, and how long it takes, is not a rule here yet. What is counted
is [what the machine keeps track of](../concepts/what-the-machine-tracks.md); the letters are
[M-A-C](../concepts/m-a-c.md).
