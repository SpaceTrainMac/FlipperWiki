---
rule: 0097
title: `EXTRA PLAYS` is a joke, and deliberately
source: FlipperArchitecture/docs/gameplay.md § 13. What the machine shows
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 13. What the machine shows](../../../FlipperArchitecture/docs/gameplay.md#13-what-the-machine-shows)

**`EXTRA PLAYS` is a joke, and deliberately.** The machine is played at home and free — when a game
ends, the next one starts — so there are no plays to owe, and a permanently dark digit says less
than a cheerful one. **The digit shows a `0`, which on seven segments is an open eye, and it
winks:**

| | Segment | For |
|---|---|---|
| at rest | `0` | 20 seconds |
| a wink | `-` | 300 ms |
| **every tenth wink**, instead | `-`, `0`, `-` | 300 ms, 200 ms, 300 ms |

So the eye blinks once every twenty seconds and blinks twice about every three and a half minutes,
which is often enough to be caught out of the corner of an eye and rare enough never to compete with
the playfield. **It is the one thing on this machine that is not a rule**: nothing lights it,
nothing reads it, and no score depends on it.
