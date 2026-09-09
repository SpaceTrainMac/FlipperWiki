---
rule: 0079
title: `BALLSENSOR_BALLCACHE` is the drain, and the way it closes says how many balls are still out
source: FlipperArchitecture/docs/gameplay.md § 12. The ball, the turn and the game
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 12. The ball, the turn and the game](../../../FlipperArchitecture/docs/gameplay.md#12-the-ball-the-turn-and-the-game)

**`BALLSENSOR_BALLCACHE` is the drain, and the way it closes says how many balls are still out.** A
returning ball reaches that contact before it reaches the store. If the store is empty the ball
rolls past into position and the contact **pulses**; if a ball is already in position the returning
one **rests on the contact** and holds it closed until one of the two is served again.

| `BALLSENSOR_BALLCACHE` | Means |
|---|---|
| a **pulse** | one ball is home and at least one is still in play — during multiball, nothing has ended |
| **closed and held** | every ball is home: this ball is over, and with none owed, so is the turn |
