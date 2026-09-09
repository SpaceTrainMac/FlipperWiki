---
rule: 0414
title: All three texts are static, and a seven-segment alphabet holds them
source: FlipperEngine/docs/states/credits.md § CreditsMachine — What is displayed
as-of: 0e97ce3
body: game
supersedes:
---
[credits.md § CreditsMachine — What is displayed](../../../FlipperEngine/docs/states/credits.md#what-is-displayed)

All three texts are static and spelled out in `src/machines/creditsMachine.cpp` — `CONTRIBUTORS`,
`QUOTES` and `BANNER`. Uppercase A–Z, digits, spaces and hyphens are what a 7-segment digit can
spell, and a test holds all of them to that: an unspellable character is not an error anywhere, it is
the fallback glyph appearing on the backglass a month later.
