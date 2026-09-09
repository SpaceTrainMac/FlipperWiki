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

**It takes two seconds, whatever the number is.** The turn score counts down to zero while your own
total counts up by the same amount, in 20 ticks of 100 ms ([0069](../../raw/rules/0069-when-the-turn-is-over-the-number-on.md)).

**A fixed number of ticks rather than a fixed step size**, because a step size that counted 915 000
out in readable pieces would take minutes, and because the end of a turn should not get slower as a
player gets better ([0070](../../raw/rules/0070-a-fixed-number-of-ticks-rather-than-a.md)).

TBC — what else ends with a turn is not a rule here yet. A turn can outlast a ball: see [the end of a ball](end-of-ball.md).
