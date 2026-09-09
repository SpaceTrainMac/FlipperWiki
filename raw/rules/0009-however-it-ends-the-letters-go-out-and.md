---
rule: 0009
title: However it ends, the letters go out and M-A-C can be spelled again.
source: FlipperArchitecture/docs/gameplay.md § 3. M-A-C
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 3. M-A-C](../../../FlipperArchitecture/docs/gameplay.md#3-m-a-c)

**However it ends, the letters go out and M-A-C can be spelled again.** Collected or expired,
`EXTRA_BALL_TOP` stops flashing and goes dark, and `MAC_LEFT`, `MAC_CENTER` and `MAC_RIGHT` go out
with it. **So M-A-C is a repeatable cycle and not a once-a-game latch**: spell the three lanes, take
`M` and `C` for as long as they can be found, spend the sequence on `A`, and start again from
nothing.
