---
rule: 0411
title: 60 seconds by default, and it is a settings key
source: FlipperEngine/docs/states/credits.md § CreditsMachine — The duration is configuration, not a constant
as-of: 0e97ce3
body: game
supersedes:
---
[credits.md § CreditsMachine — The duration is configuration, not a constant](../../../FlipperEngine/docs/states/credits.md#the-duration-is-configuration-not-a-constant)

**60 seconds by default, and it is a `settings.json` key** — `creditsSeconds`, held between
`Settings::MIN_CREDITS_SECONDS` and `MAX_CREDITS_SECONDS` (1 s and 1 h). How long a light show runs is
a choice made about the machine rather than a fact about it, which is the rule that decides what
belongs in settings at all ([architecture.md §7](../../../FlipperEngine/docs/architecture.md#7-configuration)).
