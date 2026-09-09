---
rule: 0342
title: Controls: all three buttons, each doing what its name says
source: FlipperEngine/docs/states/player-select.md § PlayerSelect — choosing the number of players
as-of: 0e97ce3
body: game
supersedes:
---
[player-select.md § PlayerSelect — choosing the number of players](../../../FlipperEngine/docs/states/player-select.md#playerselect--choosing-the-number-of-players)

**Controls.** All three buttons, each doing what its name says:

| Button | Does |
|---|---|
| `BUTTON_LEFT` | down — one fewer player |
| `BUTTON_RIGHT` | up — one more |
| `BUTTON_START` | commit; the state exits and `Play` begins |
