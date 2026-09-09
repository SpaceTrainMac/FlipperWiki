---
rule: 0101
title: `SPACE TRAIN LIFTS OFF` is a still message on the four player displays
source: FlipperArchitecture/docs/gameplay.md § 13. What the machine shows
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 13. What the machine shows](../../../FlipperArchitecture/docs/gameplay.md#13-what-the-machine-shows)

**`SPACE TRAIN LIFTS OFF` is a still message on the four player displays, and it is the only thing
on this machine that writes them while a ball is in play.** The four are a 2×2 block that the
machine reads as two rows of twelve characters, so the phrase lands one word to a display and
nothing has to scroll:

```text
   SPACE    TRAIN          player 1, player 2
   LIFTS    OFF            player 3, player 4
   X-PLAYS BALL CREDITS      MATCH — the turn score, still counting
```
