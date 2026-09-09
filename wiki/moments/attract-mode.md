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
