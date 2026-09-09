---
title: The MATCH display
type: thing
aliases: [MATCH, the MATCH display, the fifth display, the turn score display]
body: game
---
# The MATCH display

**In [the service menu](../moments/the-service-menu.md) it says `SETUP`**, and in
[the radio](../moments/the-radio.md) it says `RADIO`, or `NO NET` while the station will not
connect — which is how the glass tells you the machine is not in attract mode ([0255](../../raw/rules/0255-the-value-buttons-repeat-while-held.md), [0260](../../raw/rules/0260-the-cabinet-plays-a-radio-station-when-left-alone.md)).

**On [the cabinet](../bodies/cabinet.md) it also carries two words that mean something is wrong**
([0259](../../raw/rules/0259-two-words-on-the-match-display-mean-something-is-wrong.md)). `NOSAVE` is a settings file or a high score table that could not be written, with the old
one left alone ([0250](../../raw/rules/0250-a-failed-write-is-not-renamed-over-a-good-file.md), [0259](../../raw/rules/0259-two-words-on-the-match-display-mean-something-is-wrong.md)); `REBOOT` is a sound set that will not play until the machine is
restarted ([0259](../../raw/rules/0259-two-words-on-the-match-display-mean-something-is-wrong.md)).

**The fifth six-digit display, and during a game it is the score you are making right now** — this
turn's, not the game's ([0011](../../raw/rules/0011-ten-quantities-and-everything-below-is-one-of.md)). **So this is the display to watch while the ball is in play**:
everything you earn goes here, and [your own display](player-displays.md) does not move until the
turn is over ([0012](../../raw/rules/0012-the-score-moves-only-between-turns-and-that.md)).

**It divides by ten too, and has no lamp to say so.** A turn is a ball plus every extra ball it
earns and one ball alone can reach 915 000, so a turn passes six digits easily — there are four
`×10` indicators, one a player, and none for this display. **The turn score is not capped at
999 999; the display is** ([0099](../../raw/rules/0099-the-fifth-display-divides-by-ten-too-and.md)).

**It is where the end-of-ball count lands**, one lamp at a time, 200 ms apart ([0063](../../raw/rules/0063-one-step-per-lit-lamp-200-ms-apart.md)).

**At the end of the turn it walks back down to zero** while your own display climbs ([0069](../../raw/rules/0069-when-the-turn-is-over-the-number-on.md)), and it
is blanked once the transfer finishes — so you never walk up to the last player's number ([0075](../../raw/rules/0075-the-match-display-is-blanked-once-the-transfer.md)).

**Outside a game it is three displays in one, and the LED lit beside it says which** ([0106](../../raw/rules/0106-during-a-game-the-fifth-display-is-the.md)):

| Lit | `MATCH` is showing |
|---|---|
| `EXTRA BALL` right | the extra balls that player won across the whole game |
| `HIGH SCORE` | that player's best score |
| `EXTRA PLAY` | extra plays won — **the mode this cabinet does not use** |

*(the table is rule 0106's, rendered for a player)*

**The high-score screen and the end-of-game statistics toggle between the two it does use**, five
seconds each, moving the lamp with the number — a display that changed meaning without saying so
would be unreadable ([0107](../../raw/rules/0107-the-high-score-screen-and-the-end-of-game-statistics-toggle.md)).

At the end of a game it also carries [the draw](../moments/the-draw.md)'s two digits — the ones the
display is named for ([0091](../../raw/rules/0091-when-every-player-is-out-of-balls-the.md)), and the extra balls you won ([0011](../../raw/rules/0011-ten-quantities-and-everything-below-is-one-of.md)).

See [what the machine keeps track of](../concepts/what-the-machine-tracks.md) and
[the four player displays](player-displays.md).
