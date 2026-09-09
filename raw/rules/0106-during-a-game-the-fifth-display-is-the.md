---
rule: 0106
title: During a game the fifth display is the turn score and nothing else
source: FlipperArchitecture/docs/gameplay.md § 13. What the machine shows
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 13. What the machine shows](../../../FlipperArchitecture/docs/gameplay.md#13-what-the-machine-shows)

**During a game the fifth display is the turn score and nothing else**
([§11](../../../FlipperArchitecture/docs/gameplay.md#11-the-end-of-a-turn-the-transfer)), and at the end of one it carries the draw's two digits
([§12](../../../FlipperArchitecture/docs/gameplay.md#12-the-ball-the-turn-and-the-game)). **Between those it is three displays in one, and the
LED lit beside it says which:**

| Lit | `MATCH` is showing |
|---|---|
| `EXTRA BALL` right | the extra balls that player won across the whole game |
| `HIGH SCORE` | that player's best score |
| `EXTRA PLAY` | extra plays won — **the mode this cabinet does not use** |
