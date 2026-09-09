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
