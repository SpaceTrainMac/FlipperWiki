---
rule: 0418
title: QUOTES is shown in random order, dealt as a deck
source: FlipperEngine/docs/states/credits.md § CreditsMachine — What is displayed
as-of: 0e97ce3
body: game
supersedes:
---
[credits.md § CreditsMachine — What is displayed](../../../FlipperEngine/docs/states/credits.md#what-is-displayed)

**`QUOTES` is shown in random order, dealt as a deck.** The whole list is shuffled once, walked to
the end, and only then shuffled again — so every quote comes up before any of them comes up twice,
and a fresh deal never opens with the quote the last one closed on. A draw per quote would have been
random too, and would have left one quote unseen for a dozen games while another turned up in half of
them; on a list this short that is the difference a player notices. The generator is seeded from
`std::random_device` rather than the clock, for the reason [`Jukebox`](../../../FlipperEngine/docs/sound.md) is: a Pi has no
real-time clock, so `time(nullptr)` would deal the same "random" order after every power cycle.
