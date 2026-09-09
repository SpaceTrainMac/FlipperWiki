---
rule: 0081
title: Drain protection covers the first 15 seconds (configurable) after that shot
source: FlipperArchitecture/docs/gameplay.md § 12. The ball, the turn and the game
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 12. The ball, the turn and the game](../../../FlipperArchitecture/docs/gameplay.md#12-the-ball-the-turn-and-the-game)

**Drain protection covers the first 15 seconds (configurable) after that shot**, measured from
`OUTFIRE`. `HOUSE_BALL` flashes for that window to show it is armed — the playfield prints `EXTRA
BALL` beside that lamp, so a blinking `HOUSE_BALL` is read on the cabinet as *drain now and you
still have your ball*. **Any** drain inside the window is covered: the ball comes back on its own as
soon as the store has one staged, and the protection is spent the first time it saves a drain and
does not re-arm until that player's next turn.
