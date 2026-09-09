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

## What is on the glass

**The four player displays are read as two rows of twelve characters** ([0413](../../raw/rules/0413-two-rows-of-twelve-characters.md)):

| Row | Shows | How |
|---|---|---|
| **top** | the people who built the machine, one string | scrolling, for the whole state |
| **bottom** | one quote, then the next | scrolling, at twice the speed |
| [`MATCH`](../things/match-display.md) | `CRDTS`, still | written once |

*(the table is credits.md's, rendered for a player ([0413](../../raw/rules/0413-two-rows-of-twelve-characters.md)))*

**All three texts are fixed, and every character in them is one a seven-segment display can
actually spell** — uppercase A–Z, digits, spaces and hyphens — **which a test holds them to**
([0414](../../raw/rules/0414-all-three-texts-are-static.md)). An unspellable character would not be an error, it would be the fallback glyph turning up
on the backglass a month later ([0414](../../raw/rules/0414-all-three-texts-are-static.md)).

**The fifth display says which screen this is**, because the other two rows never stand still —
**somebody who walks up mid-quote could otherwise watch a sentence go past without learning what
they are looking at** ([0415](../../raw/rules/0415-the-fifth-display-says-which-screen-this-is.md)). It is written once on the first cycle and stays there, because
nothing else in this state touches it ([0415](../../raw/rules/0415-the-fifth-display-says-which-screen-this-is.md)).

**The top row is a ticker rather than a list** — the end of the string is followed directly by the
beginning of it, with no dark gap between the last name and the first ([0416](../../raw/rules/0416-the-top-row-is-a-ticker.md)). **Nobody should
have to arrive at the right second to see all three** ([0416](../../raw/rules/0416-the-top-row-is-a-ticker.md)).

**The names scroll at half the speed of the quotes, and both numbers follow from what each row has
to say** ([0417](../../raw/rules/0417-the-names-scroll-at-half-the-speed.md)). The top row is three names going round for a whole minute, so it can be read
slowly. **A quote is one pass of up to 120 characters across a twelve-character window, and the
roll is only a minute**: at the slow rate the longest one would take 53 seconds — nearly the whole
state for a single sentence — against 26 at the normal rate, which leaves room for a second quote
and sometimes a third ([0417](../../raw/rules/0417-the-names-scroll-at-half-the-speed.md)).

**The quotes are dealt like a deck rather than drawn at random** — the whole list is shuffled,
played to the end, and only then shuffled again ([0418](../../raw/rules/0418-quotes-are-dealt-as-a-deck.md)). **So every quote comes up before any of
them comes up twice**, and a fresh deal never opens with the quote the last one closed on ([0418](../../raw/rules/0418-quotes-are-dealt-as-a-deck.md)).
Drawing one at random each time would be random too, and would leave one quote unseen for a dozen
games while another turned up in half of them — **on a list this short that is the difference a
player notices** ([0418](../../raw/rules/0418-quotes-are-dealt-as-a-deck.md)).

**The deck carries on from one roll to the next rather than being dealt again**, so a second game
does not open with the quote the first one opened with ([0419](../../raw/rules/0419-the-deck-carries-on-between-rolls.md)).

## The light show

**The reading matter is only half of it, and the two halves are deliberately unalike** ([0420](../../raw/rules/0420-the-cabinet-is-lit-as-well.md)):

| | What it does | Why |
|---|---|---|
| [the 48 playfield lamps](../things/playfield-lamps.md) | one random lamp on and another off, every 50 ms | no pattern to spot, so it never looks like a sequence that has got stuck |
| [the RGB backlight](../things/cabinet-backlight.md) | three sine waves, at wavelengths 1 : 2 : 4 | the slowest thing on the cabinet, against the fastest |

*(the table is credits.md's, rendered for a player ([0420](../../raw/rules/0420-the-cabinet-is-lit-as-well.md)))*

**Nothing remembers which lamps are lit, and that is the whole trick** ([0421](../../raw/rules/0421-nothing-remembers-which-lamps-are-lit.md)). Two lamps are
drawn every cycle, one written on and one written off; **whether either was already in that state
does not matter to anyone** and finding out would cost a byte of state per lamp. One on and one off
per cycle **holds the playfield at roughly half lit on its own, with no counting** ([0421](../../raw/rules/0421-nothing-remembers-which-lamps-are-lit.md)).

**The backlight is three waves rather than one** — red at the shortest wavelength, green at twice
that and blue at four times ([0422](../../raw/rules/0422-the-backlight-is-three-waves.md)). Three periods in that ratio share a common multiple, **so the
colour repeats every sixteen seconds and passes through a different mix on the way each time**; one
wave on all three channels would have been a backglass pulsing white, which is a duller thing
entirely ([0422](../../raw/rules/0422-the-backlight-is-three-waves.md)). The brightness follows **elapsed time rather than a tick count**, so a machine
that runs faster does not cycle colours faster ([0422](../../raw/rules/0422-the-backlight-is-three-waves.md)).

## On the way out

**All four displays are blanked** — a roll ended by the start button ends mid-quote, and **half a
sentence standing there while the next screen comes up reads as a machine that has crashed**
([0423](../../raw/rules/0423-the-displays-are-blanked-on-the-way-out.md)).

**All 48 playfield lamps go off — not the ones this state lit, which it could not name anyway**
([0424](../../raw/rules/0424-all-48-lamps-go-off.md)). **A handful of lamps left burning is exactly what a playfield looks like with a game in
progress**, and what comes next is [player select](player-select.md), where there is none ([0424](../../raw/rules/0424-all-48-lamps-go-off.md)).

**The backlight goes to white rather than to black** ([0425](../../raw/rules/0425-the-backlight-goes-to-white.md)). Nothing but attract mode drives
these three channels, so whatever is left here stands until the light show comes round again — and
**a colour frozen wherever the wave happened to stop is an accident on the backglass, while dark is
a cabinet somebody has turned off. White is neither** ([0425](../../raw/rules/0425-the-backlight-goes-to-white.md)).

TODO — **the closing titles have no music of their own yet** ([0426](../../raw/rules/0426-the-credits-roll-has-no-music-of-its-own.md)).
[The highscore theme](../concepts/the-sounds.md) exists and is the obvious thing to play under the
roll, and the state currently starts none — **so whatever was playing when the game ended carries
on** ([0426](../../raw/rules/0426-the-credits-roll-has-no-music-of-its-own.md)).
