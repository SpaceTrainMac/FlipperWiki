---
title: Player select
type: moment
aliases: [player select, choosing the number of players, PLAYER, how many are playing]
body: game
---
# Player select

**It sits between [attract mode](attract-mode.md) and the first ball, and it has one job: how many
are playing, 1 to 4** ([0341](../../raw/rules/0341-sits-between-the-intro-and-the-first-ball.md)).

**All three buttons, each doing what its name says** ([0342](../../raw/rules/0342-player-select-controls.md)):

| Button | Does |
|---|---|
| [left flipper](../things/flipper-buttons.md) | down — one fewer player |
| [right flipper](../things/flipper-buttons.md) | up — one more |
| [start](../things/start-button.md) | commit; the state exits and the game begins |

*(the table is player-select.md's, rendered for a player ([0342](../../raw/rules/0342-player-select-controls.md)))*

**It starts at 1 and clamps at both ends** — down at 1 and up at 4 do nothing, and there is no
wrap-around ([0343](../../raw/rules/0343-the-count-clamps-at-both-ends.md)).

**Start means start** — it is what brought you here from the light show and it is what begins the
game, so there is no third meaning to learn and no separate *accept* control to find ([0344](../../raw/rules/0344-start-means-start.md)).

**Double-tapping start gives a one-player game** — the common case needs no adjusting at all:
press start to come in, press start again to play ([0345](../../raw/rules/0345-double-tapping-start-gives-one-player.md)).

**Holding a button does nothing more than pressing it** — every button on this machine reports
changes rather than levels, so one physical press is one answer and holding it down produces
nothing further ([0346](../../raw/rules/0346-all-button-handling-is-edge-triggered.md)). That is what makes reusing start safe: **the press that left the light
show cannot also commit here** ([0346](../../raw/rules/0346-all-button-handling-is-edge-triggered.md)).

## What the glass does

**The glass goes dark on the way in, and that is the first thing this state does** ([0347](../../raw/rules/0347-the-glass-is-dark-on-the-way-in.md)). Every
display group is blanked and all sixteen [LEDs](../things/indicator-leds.md) written out before
anything of its own is drawn — because **what is on the glass when this state opens belongs to
whoever was there before** ([0347](../../raw/rules/0347-the-glass-is-dark-on-the-way-in.md)). Attract mode leaves the high score table walking across the
score displays; a game that has just finished leaves four totals, `GAME OVER` and a match number,
and none of it is true while somebody is choosing how many are playing ([0347](../../raw/rules/0347-the-glass-is-dark-on-the-way-in.md)).

**The playfield lamps are not touched, and that is the line** — the light show owns them until
the game does, and blanking them here would put the machine dark at the one moment somebody is
standing in front of it ([0348](../../raw/rules/0348-the-playfield-lamps-are-not-touched.md)).

**Then it draws its own two things: the count, and the word** ([0349](../../raw/rules/0349-then-it-draws-its-own-two-things.md)).

**`PLAYER` on [the fifth display](../things/match-display.md)** — the six-digit group in the
bottom-right corner, which is free here because the turn score that owns it during a game does not
exist yet ([0350](../../raw/rules/0350-player-on-the-fifth-display.md)). It says what the corner of the glass is counting, and it goes out again with
the count on the way out ([0350](../../raw/rules/0350-player-on-the-fifth-display.md)).

**The count is shown in two places at once** — as a digit on [the status row](../things/status-row.md)'s
left-hand position, and as one to four of the [player-active lamps](../things/indicator-leds.md)
lit beside it ([0351](../../raw/rules/0351-showing-the-count-in-two-places-at-once.md)). **The digit *counts* and the lamps *show*,** which are the two places a
player already looks during a game ([0351](../../raw/rules/0351-showing-the-count-in-two-places-at-once.md)). That digit is free here for the same reason
`BALL IN PLAY` is: no ball is in play, and no extra balls have been won in a game that has not
started ([0351](../../raw/rules/0351-showing-the-count-in-two-places-at-once.md)).

**All four lamps are written on every change rather than just the one that moved** — stepping down
from three to two has to put a lamp *out*, and a draw that only ever lights things cannot ([0352](../../raw/rules/0352-all-four-lamps-are-written-on-every-change.md)).
