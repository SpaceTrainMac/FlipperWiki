---
title: Lit awards, and how they are collected
type: concept
aliases: [lit awards, lights versus gives, collecting an award]
body: game
---
# Lit awards, and how they are collected

**A lit lamp is an award waiting for you to go and get it.** *Lights* an award and *gives* an award
are two different things on this machine: a lamp that is lit stays lit until the switch that
collects it closes, or until the ball ends ([0018](../../raw/rules/0018-the-lit-awards-wait-to-be-collected-which.md)).

| Award | Lit by | Collected at |
|---|---|---|
| [`SPECIAL`](../things/special-lamps.md), both lamps | M-A-C completing, or the bank's 3rd completion | [either outlane](../things/outlanes.md) |
| [the upper `EXTRA BALL`](../things/upper-target-bank.md) | `A`, with M-A-C complete — a 20-second window | [the right captive ball](../things/right-captive-ball.md) |
| [the right `EXTRA BALL`](../things/extra-ball-right.md) | the bank's 2nd completion, and nothing else — it stays lit until collected | [the right captive ball](../things/right-captive-ball.md) |
| [`HOLE BONUS 30000`](../things/hole-bonus-ladders.md), per side | that side's ladder reaching its 5th hit, or the right captive ball | that side's own bunker, or the end of the ball |

*(the table is rule 0018's, rendered for a player)*

**Four awards do not wait: they are lit on a timer, and a window that closes uncollected pays
nothing at all** ([0019](../../raw/rules/0019-four-awards-are-lit-on-a-timer-instead.md)).

| On a timer | Runs for | The lamp |
|---|---|---|
| [the upper `EXTRA BALL`](../things/upper-target-bank.md), after `A` | 20 s | `EXTRA_BALL_TOP` with the `A` lamp |
| [the extra bonus](../things/x-bon-lamp.md), at the 40th and 50th completion | 20 s | `X_BON` |
| a [hole-bonus](../things/hole-bonus-ladders.md) redemption, either side | 30 s | that side's five rungs with its `HOLE BONUS 30000` |
| [drain protection](../things/house-ball-lamp.md) | 15 s | `HOUSE_BALL` |

*(the table is rule 0019's, rendered for a player)*
