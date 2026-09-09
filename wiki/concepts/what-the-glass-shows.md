---
title: What the glass shows
type: concept
aliases: [the displays, what the displays show, the backglass]
body: game
---
# What the glass shows

**Six things are written above the playfield, and only two of them are your score** ([0093](../../raw/rules/0093-the-displays.md)):

| Display | During a game |
|---|---|
| [the four six-digit player scores](../things/player-displays.md) | that player's total **as it stood when their turn began**; it moves only during a transfer |
| [the fifth six-digit display, `MATCH`](../things/match-display.md) | the **turn score** — zero when the turn begins, blanked when it ends |
| [`BALL IN PLAY`](../things/status-row.md) | **turns left, counting down**, including the one being played |
| [the two-digit field](../things/status-row.md) | **extra balls in hand** — one up per award, one down per drain |
| [`EXTRA PLAYS`](../things/extra-plays-eye.md) | a `0` that winks — an eye, not a number |
| two digits between them | **dark** — the backglass artwork covers them |

*(the table is rule 0093's, rendered for a player)*

**Every digit is seven segments, and the machine sends segments rather than numbers** — which is
why it can spell at all, and why a word it spells badly is a limit of seven segments rather than of
the machine ([0241](../../raw/rules/0241-a-digit-is-seven-segments.md)). [The simulator](../bodies/simulator.md) lights them from the same bytes the
engine puts on the wire ([0241](../../raw/rules/0241-a-digit-is-seven-segments.md)).

**They are green.** Every photograph of this cabinet shows green digits, and
[the VPX table](../bodies/vpx.md) draws them green for that reason ([0224](../../raw/rules/0224-the-displays-are-green.md)). **On that body the panel
is redrawn and deliberately too wide**: at the cabinet's real proportions a six-digit score would
stand about 19 pixels tall, which is not a score anybody could read ([0233](../../raw/rules/0233-the-backbox-is-drawn-not-photographed.md)).
