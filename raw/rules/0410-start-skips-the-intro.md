---
rule: 0410
title: Start skips the intro
source: FlipperEngine/docs/states/credits.md § CreditsMachine — the closing titles
as-of: 0e97ce3
body: game
supersedes:
---
[credits.md § CreditsMachine — the closing titles](../../../FlipperEngine/docs/states/credits.md#creditsmachine--the-closing-titles)

**Start skips the intro.** Someone watching the names who presses start has already decided to play
again, and sending them through attract mode first would make them wait for a screen they just chose
to leave. This is the only route into a game that does not pass through `Intro`, and it is why the
transition table gives this state a real choice where `Highscore` and `Setup` have exactly one way
out.

The press is edge-triggered like every other button on the machine
([`PlayerSelect`](../../../FlipperEngine/docs/states/player-select.md)), so the press that finished name entry in
`Highscore` cannot also skip the credits.
