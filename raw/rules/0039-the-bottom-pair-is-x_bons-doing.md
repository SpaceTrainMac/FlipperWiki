---
rule: 0039
title: The bottom pair is `X_BON`'s doing
source: FlipperArchitecture/docs/gameplay.md § 7. The three multipliers
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 7. The three multipliers](../../../FlipperArchitecture/docs/gameplay.md#7-the-three-multipliers)

**The bottom pair is `X_BON`'s doing.** `X_BON` — the `X BONUS` target printed on the lower
playfield — lights and flashes for a configurable 20 seconds the moment the hidden total-completions
count from [§5](../../../FlipperArchitecture/docs/gameplay.md#5-the-bonus-count) reaches 40. Hitting the right captive ball
(`BALLWITHBALL_RIGHT_TOP`) inside that window releases the *extra bonus*: its own sound and light
cue, a flat **500 000**, and `X2_BOT` lights. The same happens again at the 50th total completion,
`X_BON` flashing for the same window a second time, and a collection inside it lights `X3_BOT`
instead — the ceiling, whether or not `X2_BOT` was ever lit. A window that closes uncollected costs
the player the 500 000 and the multiplier both.
