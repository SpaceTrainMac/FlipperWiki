---
rule: 0409
title: Two exits
source: FlipperEngine/docs/states/credits.md § CreditsMachine — the closing titles
as-of: 0e97ce3
body: game
supersedes:
---
[credits.md § CreditsMachine — the closing titles](../../../FlipperEngine/docs/states/credits.md#creditsmachine--the-closing-titles)

**Two exits**, and like every other machine below the top level it reports how it ended rather than
choosing where control goes ([the intended top level](../../../FlipperEngine/docs/state-machines.md#1-top-level--intended)):

| Exit | Reported | Top level goes to |
|---|---|---|
| `BUTTON_START` | `CREDITS_PLAYER_SELECT` (0) | `PlayerSelect` |
| the duration elapses | `CREDITS_TIMEOUT` (-1) | `Intro` |
