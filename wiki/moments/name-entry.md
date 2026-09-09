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
