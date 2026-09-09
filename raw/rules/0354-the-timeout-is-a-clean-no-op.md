---
rule: 0354
title: The timeout is a clean no-op
source: FlipperEngine/docs/states/player-select.md § PlayerSelect — choosing the number of players
as-of: 0e97ce3
body: game
supersedes:
---
[player-select.md § PlayerSelect — choosing the number of players](../../../FlipperEngine/docs/states/player-select.md#playerselect--choosing-the-number-of-players)

**The timeout is a clean no-op** — the machine returns to the intro as if nothing had happened, so a
cabinet nudged in an empty room does not sit in select mode indefinitely. Nothing is consumed and
nothing needs undoing, and that falls out of where the commit point is: credits would be charged
**per player**, so the machine cannot know how many to debit until `numPlayers` is confirmed. That
makes `BUTTON_START` the commit point by definition, and a timeout happens strictly before it.
