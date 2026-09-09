---
title: Attract mode
type: moment
aliases: [attract mode, the attract, the intro, the light show, the ladder, the high score scene]
body: game
---
# Attract mode

**A light show that runs until somebody presses start, and it is where this cabinet spends nearly
all of its life** ([0325](../../raw/rules/0325-attract-mode-runs-until-someone-presses-start.md)).

**It is one state with two scenes, shown in turn** — a climbing light show, and the high score
table ([0326](../../raw/rules/0326-one-state-two-scenes.md)).

## The ladder

**What moves is a horizontal line, and it crosses the whole cabinet** ([0327](../../raw/rules/0327-a-horizontal-line-crossing-the-whole-cabinet.md)). The rise starts at
the drain at the bottom of the playfield, climbs row by row, carries on up into the backglass and
stops at the M-A-C lanes' equivalent up there — the player 1 and 2 score displays at the top of
the panel. Then it comes back down the same way ([0327](../../raw/rules/0327-a-horizontal-line-crossing-the-whole-cabinet.md)).

**The playfield is walked in rows rather than in wiring order** — lamps are grouped by how high
up the playfield they sit, so [three lamps within ten units of each other](../things/playfield-lamps.md)
light on the same step ([0328](../../raw/rules/0328-the-playfield-is-walked-in-rows.md)). **The sequence this replaced climbed one bank and then dropped
back down to start again** ([0328](../../raw/rules/0328-the-playfield-is-walked-in-rows.md)).

**The backglass rises too, and its bands interleave** — four rows of
[LEDs](../things/indicator-leds.md) and three of [display groups](../concepts/what-the-glass-shows.md),
with [the status row](../things/status-row.md) *below* the player scores rather than beside them
([0329](../../raw/rules/0329-the-backglass-rises-too.md)).

**A display row is five steps of the animation rather than one** ([0330](../../raw/rules/0330-a-display-row-is-five-steps.md)). A digit is tall enough
that a line crossing it is six shapes in order — a blank, `_`, `u`, `o`, an upside-down `A`, and
back — and **nothing else on the glass moves while that happens**; on the way down a row drains
to blank completely before the row below starts ([0330](../../raw/rules/0330-a-display-row-is-five-steps.md)).

**Every 7-segment digit on the backglass takes part, and all sixteen LEDs with them** ([0331](../../raw/rules/0331-every-digit-takes-part.md)).

## The high score scene

**The lamps do not stop** ([0332](../../raw/rules/0332-the-lamps-do-not-stop.md)). The playfield still climbs row by row, the backglass LEDs climb
with it and the backlight still fades — all of that is identical to the ladder. **What changes is
that the 7-segment displays are taken out of the climb and given over to the table** ([0332](../../raw/rules/0332-the-lamps-do-not-stop.md)).

**Two entries are on the glass at once, and the window slides from the worst place towards the
best** — 9th over 10th, then 8th over 9th, ending on 1st over 2nd: nine pages for a full table of
ten ([0333](../../raw/rules/0333-the-window-slides-from-worst-to-best.md)). **Every page but the ends shows a name twice**, once arriving at the bottom and once
moving up, which is what makes it read as one list travelling rather than nine unrelated screens —
and **ending on first place leaves the score to beat as the last thing on the glass** ([0333](../../raw/rules/0333-the-window-slides-from-worst-to-best.md)).
Each entry sits across one row of two displays, the name on the left and the score on the right,
with `SCORES` on [`MATCH`](../things/match-display.md) throughout ([0333](../../raw/rules/0333-the-window-slides-from-worst-to-best.md)).

**The table is copied once when the scene opens**, so a game finishing mid-scroll cannot renumber
the list under whoever is reading it — and a table with fewer than two entries makes no window at
all ([0334](../../raw/rules/0334-the-table-is-copied-once-when-the-scene-opens.md)).

**Two rates come off one clock, and that is why it looks the way it does** ([0335](../../raw/rules/0335-two-rates-off-one-clock.md)). The beat is
50 ms: [the backlight](../things/cabinet-backlight.md) fades on every beat, which is what a 64-step
colour ramp wants, and the lamps and displays advance every *second* beat, which is what makes the
line travelling up the cabinet followable rather than a flicker ([0335](../../raw/rules/0335-two-rates-off-one-clock.md)).

## The two gestures

**There is no service button on this cabinet** — all 32 matrix inputs are
[playfield switches](../things/every-switch.md) or [the three buttons](../things/flipper-buttons.md) —
so both things that can be asked for that are not a game are gestures on the flippers ([0336](../../raw/rules/0336-no-service-button-so-two-gestures.md)):

| Hold | For nine seconds | Gets you |
|---|---|---|
| **both flippers** | with a headline and a countdown on the glass | [the service menu](the-service-menu.md) |
| **the right flipper alone** | with its own tease | [the radio](the-radio.md) |

*(the table is intro.md's, rendered for a player ([0336](../../raw/rules/0336-no-service-button-so-two-gestures.md)))*

**Both are nine seconds on purpose** — two holds on the same buttons running to different lengths
would be two things to learn, and one of them would be got wrong every time ([0337](../../raw/rules/0337-the-radio-gesture-is-the-same-nine-seconds.md)). The radio
gesture exists because the alternative was waiting: the radio arrives by itself after a set idle,
which is right for a cabinet nobody is standing at and useless to somebody standing at it who wants
it on now ([0337](../../raw/rules/0337-the-radio-gesture-is-the-same-nine-seconds.md)).

**On a cabinet with no radio the gesture does nothing and the tease never comes up** — it is armed
by the same setting that arms the wait, so a machine with no stations, or with its sound switched
off, simply does not have it ([0338](../../raw/rules/0338-the-gesture-is-armed-by-the-same-number-as-the-wait.md)).

**Neither gesture can be mistaken for the other, and it takes two rules rather than one** ([0339](../../raw/rules/0339-neither-gesture-can-be-mistaken-for-the-other.md)).
Two hands do not close two switches in the same millisecond, so a solo hold is only counted after
the other button has been genuinely up for a moment — **and any hold the other flipper was seen
down during is out for good until that button is released** ([0339](../../raw/rules/0339-neither-gesture-can-be-mistaken-for-the-other.md)). The second rule is the one
that is easy to miss: without it, letting go of one hand halfway through the service gesture would
start a nine-second countdown to the radio ([0339](../../raw/rules/0339-neither-gesture-can-be-mistaken-for-the-other.md)).

**An abandoned gesture is ignored rather than acted on** ([0340](../../raw/rules/0340-an-abandoned-gesture-is-ignored.md)). The tease goes up at three
seconds; let go before the nine are out and the light show starts moving again, but **the text is
left on the glass until the end of the next run up or down** — taking it away at the instant of
release would take it from somebody who is still reading it ([0340](../../raw/rules/0340-an-abandoned-gesture-is-ignored.md)). That is the whole reason
there is a warning six seconds before anything happens at all ([0340](../../raw/rules/0340-an-abandoned-gesture-is-ignored.md)).
