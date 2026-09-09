---
rule: 0353
title: Two exits
source: FlipperEngine/docs/states/player-select.md § PlayerSelect — choosing the number of players
as-of: 0e97ce3
body: game
supersedes:
---
[player-select.md § PlayerSelect — choosing the number of players](../../../FlipperEngine/docs/states/player-select.md#playerselect--choosing-the-number-of-players)

**Two exits.** This machine does not choose where control goes next — it reports *how* it ended and
the top level routes it ([the intended top level](../../../FlipperEngine/docs/state-machines.md#1-top-level--intended)):

| Exit | Reported | Top level goes to |
|---|---|---|
| `BUTTON_START` | `numPlayers` = 1…4 | `Play` |
| 60 s with no button press | abandoned | `Intro` |
