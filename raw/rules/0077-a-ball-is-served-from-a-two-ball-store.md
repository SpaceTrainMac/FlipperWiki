---
rule: 0077
title: A ball is served from a two-ball store, one at a time, and four contacts watch it round
source: FlipperArchitecture/docs/gameplay.md § 12. The ball, the turn and the game
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 12. The ball, the turn and the game](../../../FlipperArchitecture/docs/gameplay.md#12-the-ball-the-turn-and-the-game)

**A ball is served from a two-ball store, one at a time, and four contacts watch it round:**

| Contact | Sees |
|---|---|
| `BALLSENSOR_BALLEJECTOR` | a ball **available to serve**. While it is closed, `FCA_1_BALL_OUT` can fire, and it reliably puts a ball in the start ramp |
| `BALLSENSOR_STARTRAMP` | that ball **arrive** in the start ramp — the sensor's own name is *vor Startrampe* |
| `OUTFIRE` | it **leave** the ramp into play — *"Out Fire" nach Startrampe*. This is the ball becoming one in play, and it opens the drain-protection window below |
| `BALLSENSOR_BALLCACHE` | a ball **come back**. It is the drain |
