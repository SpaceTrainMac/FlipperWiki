---
title: The ball store, and the four contacts
type: thing
aliases: [the ball store, the trough, BALLSENSOR_BALLEJECTOR, BALLSENSOR_STARTRAMP, BALLSENSOR_BALLCACHE, the two-ball store]
body: game
---
# The ball store, and the four contacts

**A ball is served from a two-ball store, one at a time, and four contacts watch it round** ([0077](../../raw/rules/0077-a-ball-is-served-from-a-two-ball-store.md)):

| Contact | Sees |
|---|---|
| `BALLSENSOR_BALLEJECTOR` | a ball **available to serve** — while it is closed the ejector can fire, and it reliably puts a ball in the start ramp |
| `BALLSENSOR_STARTRAMP` | that ball **arrive** in the start ramp |
| [`OUTFIRE`](outfire.md) | it **leave** the ramp into play — the ball becoming one in play, and the start of the drain-protection window |
| `BALLSENSOR_BALLCACHE` | a ball **come back**. It is the drain |

*(the table is rule 0077's, rendered for a player)*

**The drain contact says how many balls are still out, by how it closes.** A returning ball reaches
it before it reaches the store: if the store is empty the ball rolls past into position and the
contact **pulses**; if a ball is already in position the returning one **rests on it** and holds it
closed until one of the two is served again ([0079](../../raw/rules/0079-ballsensor_ballcache-is-the-drain-and-the-way-it.md)).

| `BALLSENSOR_BALLCACHE` | Means |
|---|---|
| a **pulse** | one ball is home and at least one is still in play — during multiball, nothing has ended |
| **closed and held** | every ball is home: this ball is over, and with none owed, so is the turn |

*(the table is rule 0079's, rendered for a player)*

**A saved ball waits on the store, not on the drain** — the ball has to roll the length of the
trough before the ejector has anything to fire ([0083](../../raw/rules/0083-what-the-machine-waits-for-instead-is-a.md)).

**Which is why nothing on this machine counts balls in play.** Two balls and two positions in the
store make a held contact the whole answer, and a machine that could not tell one returning ball
from two would have needed a counter it has no switch to keep honest ([0080](../../raw/rules/0080-which-is-why-nothing-on-this-machine-counts.md)).
