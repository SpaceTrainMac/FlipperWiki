---
title: Name entry
type: moment
aliases: [name entry, entering your initials, recording the scores, typing your name, the rub-out]
body: game
---
# Name entry

**It is entered after every game, whether or not anybody earned a place** ([0383](../../raw/rules/0383-highscore-is-entered-after-every-game.md)). Whether anyone
did is decided inside it, and it passes straight through when nobody did — so **one piece of code
knows what qualifying means**, rather than the question being asked in two places ([0383](../../raw/rules/0383-highscore-is-entered-after-every-game.md)).

**On most games it does nothing at all and returns in about a millisecond** — a cabinet played for
a week has ten rows that are hard to beat, and a decision that has decided *no* has nothing to say
([0384](../../raw/rules/0384-it-is-a-decision-point-not-a-screen.md)). **The state after it is a minute of closing titles, and that is where a game's ending
belongs** ([0384](../../raw/rules/0384-it-is-a-decision-point-not-a-screen.md)).

## Who qualifies

**The test is a merge, and it is answered once, on the way in** ([0385](../../raw/rules/0385-the-merge-is-the-test.md)). The table as it stands,
plus the game's scores in player order, sorted and trimmed to ten — **a player qualifies if and
only if their row survives that, and their place is the row it is standing in** ([0385](../../raw/rules/0385-the-merge-is-the-test.md)). It is
deliberately the same arithmetic that writes the table afterwards, so the place on the glass and
the table on disk are one calculation rather than two that have to agree ([0385](../../raw/rules/0385-the-merge-is-the-test.md)).

**Beating the bottom row is not a place — surviving the trim is** ([0386](../../raw/rules/0386-beating-the-bottom-row-is-not-a-place.md)), and the two stop being
the same thing the moment two players qualify in one game: on a default table, four players on
1 100, 1 200, 1 300 and 1 400 each beat the bottom row, and fourteen rows trimmed to ten keep one of
them ([0386](../../raw/rules/0386-beating-the-bottom-row-is-not-a-place.md)).

**It is not asked again between players** — writing the first player's row could otherwise
displace the second, **which would decide who gets into the table by who typed first** ([0387](../../raw/rules/0387-qualifying-is-not-asked-again-between-players.md)).

**The order is player order — 1, 2, 3, 4, skipping the ones who did not qualify** ([0388](../../raw/rules/0388-the-order-is-player-order.md)). By
score was the alternative and it loses on the only ground that matters at a cabinet: **the player
has to know it is their turn**, and *best first* is a comparison the machine would be making at
them ([0388](../../raw/rules/0388-the-order-is-player-order.md)). Nothing is hidden by it, because [`MATCH`](../things/match-display.md) says the
place anyway ([0388](../../raw/rules/0388-the-order-is-player-order.md)).

## Typing a name

**Six characters, on the entering player's own six-digit display** — the one that has been showing
their score all game ([0389](../../raw/rules/0389-six-characters-on-the-players-own-display.md)). **The other three keep their final scores**, so the result stays
readable while somebody is typing ([0389](../../raw/rules/0389-six-characters-on-the-players-own-display.md)).

**The alphabet is a ring of thirty-nine positions, walked in both directions and wrapping at both
ends** ([0390](../../raw/rules/0390-the-ring-of-thirty-nine-positions.md)):

```text
   [rub out]  [space]  A B C … Z  0 1 2 … 9  -
```

| Button | Does |
|---|---|
| [left flipper](../things/flipper-buttons.md) | the previous position in the ring |
| [right flipper](../things/flipper-buttons.md) | the next one |
| [start](../things/start-button.md) | confirms the character and moves along one |

*(the ring and the table are highscore.md's, rendered for a player ([0390](../../raw/rules/0390-the-ring-of-thirty-nine-positions.md)))*

**It is the same three buttons doing the same three jobs as [player select](player-select.md) and
[the service menu](the-service-menu.md)**, which is why there is one interaction model on this
machine and not three ([0391](../../raw/rules/0391-the-same-three-buttons-doing-the-same-jobs.md)). **Auto-repeat is not optional** — a held button reports one edge
— so it is built, and shared with the menu ([0391](../../raw/rules/0391-the-same-three-buttons-doing-the-same-jobs.md)).

**Each character opens where the previous one was confirmed**, so `AAA` and `FFF` are three presses
of start with no stepping at all ([0392](../../raw/rules/0392-each-character-opens-where-the-last-was-confirmed.md)).

**The first character of every name opens on `A`** — one step from the space and two from the
rub-out ([0393](../../raw/rules/0393-the-first-character-opens-on-a.md)).

**A name is ended by walking to the space** — after which every remaining character is one press
of start. **There is no fourth button, so there is no *done* gesture to discover** ([0394](../../raw/rules/0394-a-name-is-ended-by-walking-to-the-space.md)).

**The first position on the ring is a rub-out** — it moves *back* one character, discards what was
there, and stays on the rub-out ([0395](../../raw/rules/0395-the-first-ring-position-is-a-rub-out.md)). So **a held start walks back through the whole name and
stops dead at the first character**, where it does nothing; start auto-repeats there and **nowhere
else**, because held on a letter it would finish a name before the player let go ([0395](../../raw/rules/0395-the-first-ring-position-is-a-rub-out.md)).

**Trailing spaces are trimmed on commit, and only the trailing ones** — `MR T` is three letters
and a gap, and it survives ([0396](../../raw/rules/0396-six-bytes-and-trailing-spaces-trimmed.md)).

## What is on the glass

**Five things, and four of them are about somebody else** ([0397](../../raw/rules/0397-what-is-on-the-glass-during-name-entry.md)):

| What | Where | Shows |
|---|---|---|
| the name being typed | [that player's own display](../things/player-displays.md) | the confirmed characters, and the one being edited |
| the other players' scores | their own displays | untouched, as the game left them |
| the place being recorded | [`MATCH`](../things/match-display.md) | `1ST`, `2ND` … `10TH` |
| whose turn | [the player-active lamps](../things/indicator-leds.md) | one lit |
| what this is | the `HIGH SCORE` lamp | lit for the whole state |

*(the table is highscore.md's, rendered for a player ([0397](../../raw/rules/0397-what-is-on-the-glass-during-name-entry.md)))*

**The character being edited blinks, and it goes back to lit on every keypress** — so the
character you have just stepped to is on the instant you get there rather than possibly starting
dark ([0398](../../raw/rules/0398-the-character-being-edited-blinks.md)).

## How an entry ends

**Three ways, and all three record something** ([0399](../../raw/rules/0399-the-three-ways-an-entry-ends.md)):

| Exit | What is recorded |
|---|---|
| the sixth character confirmed | the six characters |
| nobody pressing anything for the timeout | **what is on the glass** — the confirmed characters |
| the machine being switched off | the same |

*(the table is highscore.md's, rendered for a player ([0399](../../raw/rules/0399-the-three-ways-an-entry-ends.md)))*

**The timeout commits rather than discards, which is what makes it defensible** — the objection to
having one at all was that it could only take away a place already won, and this one does not
([0400](../../raw/rules/0400-the-timeout-commits-rather-than-discards.md)). What it buys is that **the cabinet is never stranded out of attract mode with a
half-typed name standing on the glass** ([0400](../../raw/rules/0400-the-timeout-commits-rather-than-discards.md)). Ten minutes by default, and
[an owner can change it](../bodies/cabinet.md): the timeout is not there to hurry anybody, and a
name rushed off the glass mid-word is worse than a cabinet that takes a while to notice an empty
room ([0400](../../raw/rules/0400-the-timeout-commits-rather-than-discards.md)).

**A player who walks off at the very start is recorded as `A`** — honest, and not a blank row that
reads like a fault ([0401](../../raw/rules/0401-a-player-who-walks-off-is-recorded-as-a.md)).

**The table is written after every name rather than once at the end** — four names is four writes,
which buys the property that **a power cut after the second player keeps the first two** ([0402](../../raw/rules/0402-a-failed-write-is-not-the-error-state.md)).
And **a write that fails is not an error state**: [`NOSAVE`](../things/match-display.md) goes on
`MATCH` in place of the place, and the machine carries on — a cabinet that cannot save a name
still plays pinball ([0402](../../raw/rules/0402-a-failed-write-is-not-the-error-state.md)).

**There is no music of its own here** — [the highscore theme](../concepts/the-sounds.md) belongs
to the closing titles, which are long enough to carry it ([0403](../../raw/rules/0403-no-special-music-during-name-entry.md)). **One bumper sound per
*confirmed* character, and silence while stepping** ([0403](../../raw/rules/0403-no-special-music-during-name-entry.md)).

**The `HIGH SCORE` lamp and [the knocker](../things/knocker.md) that fire mid-ball are not this
state's** — they go off the moment the best score on the cabinet changes hands, which is a
question about a game in progress ([0404](../../raw/rules/0404-the-announcement-during-a-ball-is-not-this-states.md)).

**`GAME OVER` is not this state's either** — it names the end of a *game*, which
[the state that ran it](game-over.md) knows and this one only inherits ([0405](../../raw/rules/0405-game-over-is-not-this-states.md)).
