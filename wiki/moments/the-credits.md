---
title: The closing titles
type: moment
aliases: [the credits, the closing titles, the credits roll, CRDTS, the quotes]
body: game
---
# The closing titles

**The last thing a game shows.** It rolls the names of the people who built the machine for about a
minute and then hands the cabinet back to [attract mode](attract-mode.md) — **unless somebody
presses start, in which case the next game begins immediately** ([0407](../../raw/rules/0407-the-last-thing-a-game-shows.md)).

**These are not credits in the coin sense** — coin handling is
[out of scope](player-select.md) and this state touches none of the four credit addresses on the
backglass. **One word, two meanings, and only this one is built** ([0408](../../raw/rules/0408-not-credits-in-the-coin-sense.md)).

**Two exits** ([0409](../../raw/rules/0409-credits-two-exits.md)):

| Exit | Where it goes |
|---|---|
| start | straight into [player select](player-select.md) — a new game |
| the minute elapsing | back to [attract mode](attract-mode.md) |

*(the table is credits.md's, rendered for a player ([0409](../../raw/rules/0409-credits-two-exits.md)))*

**Start skips the light show entirely, and it is the only route into a game that does** ([0410](../../raw/rules/0410-start-skips-the-intro.md)).
Somebody watching the names who presses start has already decided to play again, and sending them
through attract mode first would make them wait for a screen they have just asked to leave
([0410](../../raw/rules/0410-start-skips-the-intro.md)). The press is edge-triggered like every other on the machine, so **the press that finished
a name cannot also skip the credits** ([0410](../../raw/rules/0410-start-skips-the-intro.md)).

**Sixty seconds by default, and [an owner can change it](../bodies/cabinet.md)** — anything from a
second to an hour. **How long a light show runs is a choice made about the machine rather than a
fact about it**, which is the rule that decides what belongs in a setting at all ([0411](../../raw/rules/0411-sixty-seconds-by-default.md)).

**A value outside the range is clamped and warned about rather than refused** — exactly as a
volume of 150 is ([0412](../../raw/rules/0412-the-credits-duration-is-clamped-and-warned.md)). Both ends are real mistakes to make by hand: **a zero would make the
state a flicker nobody could read, and a value in days would park the cabinet in it looking broken**
([0412](../../raw/rules/0412-the-credits-duration-is-clamped-and-warned.md)).
