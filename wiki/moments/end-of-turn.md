---
title: The end of a turn
type: moment
aliases: [the end of a turn, the transfer, when the turn is over]
body: game
---
# The end of a turn

**This is when the two numbers meet: what you made this turn goes onto your own score.** During the
ball your display holds the total you had when the turn began and everything you earn sits on
[the `MATCH` display](../things/match-display.md); the turn ending is what moves it ([0012](../../raw/rules/0012-the-score-moves-only-between-turns-and-that.md)).

**On [the VPX table](../bodies/vpx.md) the ceremonies of a whole game come to about 43 seconds, at
real speed, with the ball in the trough throughout** — which reads differently on a screen than it
does with a ball in your hand ([0231](../../raw/rules/0231-the-bonus-and-the-match-take-about-43-seconds.md)).

**It takes two seconds, whatever the number is.** The turn score counts down to zero while your own
total counts up by the same amount, in 20 ticks of 100 ms ([0069](../../raw/rules/0069-when-the-turn-is-over-the-number-on.md)).

**The count is per ball and the transfer is per turn**, which is what makes an extra ball behave
the way you expect: the ball that just ended is counted out, the playfield is cleared, a fresh ball
is served, and everything earned across all of it moves to your display once, at the end ([0092](../../raw/rules/0092-the-count-is-per-ball-and-the.md)).

**The `MATCH` display is blanked once the transfer has finished**, so the next player never walks
up to the last player's number ([0075](../../raw/rules/0075-the-match-display-is-blanked-once-the-transfer.md)).

**The whole ceremony between turns is 2.0 to 6.8 seconds** — [the count](end-of-ball.md) and then
the transfer. Twelve turns of a four-player game at the quiet figure is about **43 seconds** of
ceremony in one game ([0074](../../raw/rules/0074-the-whole-end-of-turn-ceremony-is-between-20-s.md)).

**Nothing is announced during a ball.** Your own total does not move while you are playing, so
there is nothing to cross until the transfer — the announcement lands in the gap between turns, as
punctuation rather than as an interruption ([0073](../../raw/rules/0073-nothing-is-announced-during-a-ball.md)).

**[The knocker](../things/knocker.md) fires during the transfer**, at the tick where your climbing
total passes the standing record — first place only, once per player per game, and nothing at all
for entering the table lower down ([0072](../../raw/rules/0072-the-knocker-fires-during-the-transfer.md)).

**The two numbers together never change.** At every tick, the turn score plus your total is exactly
what it was before the transfer began, so nothing can be lost or paid twice in the middle of it — and
a transfer cut short by the cabinet being switched off finishes in one step, without the animation
([0071](../../raw/rules/0071-the-two-numbers-together-never-change.md)).

**A fixed number of ticks rather than a fixed step size**, because a step size that counted 915 000
out in readable pieces would take minutes, and because the end of a turn should not get slower as a
player gets better ([0070](../../raw/rules/0070-a-fixed-number-of-ticks-rather-than-a.md)).

A turn can outlast a ball: see [the end of a ball](end-of-ball.md).

## What changes at each edge

**A turn has two edges and the glass moves at both** ([0359](../../raw/rules/0359-initnewround-is-not-the-turns-edge.md)):

| | a ball goes into play | no ball is in play |
|---|---|---|
| counters | one ball spent, one ball played | — |
| backglass | `GAME OVER` out; [that player's lamp](../things/indicator-leds.md) lit; **`BALL IN PLAY` counted down** | that player's lamp out |
| playfield | game state reset, the flippers armed, the ball served | the timers stopped, [all 48 lamps out](../things/playfield-lamps.md) |

*(the table is game.md's, rendered for a player ([0359](../../raw/rules/0359-initnewround-is-not-the-turns-edge.md)))*

**Starting a fresh ball is not the same as starting a turn, and the difference is
[`BALL IN PLAY`](../things/status-row.md)** — an extra ball must not step it and a regular turn
must ([0359](../../raw/rules/0359-initnewround-is-not-the-turns-edge.md)).

**Each player's own lamp is lit at the start of their turn and out at the end of it** — nothing
writes all four, so **a two-player game never touches lamps 3 and 4 at all** ([0360](../../raw/rules/0360-the-active-player-lamp-is-the-players-own.md)).

**A player's score is written to their display when it changes, not on every cycle** — and it is
written once for every player as the game is set up, **so everybody reads `0` from the first ball
rather than whatever the last game left there** ([0361](../../raw/rules/0361-the-score-reaches-the-display.md)).

**The playfield goes dark when the turn ends, and it is a blunt sweep on purpose** — all 48 lamps
out, after the games' own demands have been taken and the timers cleared ([0362](../../raw/rules/0362-the-playfield-goes-dark-when-the-turn-ends.md)). Several
mechanics reset by *discarding* their pending lamp changes rather than by issuing the opposite
ones, so **without the sweep a lamp lit on one ball would carry into the next player's** ([0362](../../raw/rules/0362-the-playfield-goes-dark-when-the-turn-ends.md)).
It also settles a lamp left mid-blink, whose blink timer has just been thrown away ([0362](../../raw/rules/0362-the-playfield-goes-dark-when-the-turn-ends.md)).
