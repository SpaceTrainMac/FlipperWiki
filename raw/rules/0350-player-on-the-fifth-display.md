---
rule: 0350
title: PLAYER on the fifth display
source: FlipperEngine/docs/states/player-select.md § PlayerSelect — choosing the number of players
as-of: 0e97ce3
body: game
supersedes:
---
[player-select.md § PlayerSelect — choosing the number of players](../../../FlipperEngine/docs/states/player-select.md#playerselect--choosing-the-number-of-players)

**`PLAYER` on the fifth display.** `FDLA_DISP6_SCORE_MATCH` (158) is the six-digit group that is
adjacent to nothing six wide, which is why every state with one word to say uses it, and it is free
here — the turn score that owns it during a game does not exist yet. It says what the digit in the
corner of the glass is counting. It goes out again with the count on the way out: `Play` would
overwrite it, and the timeout back to `Intro` would not.
