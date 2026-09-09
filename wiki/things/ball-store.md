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
