---
rule: 0244
title: The operator's choices live in settings.json, not on the command line
source: FlipperEngine/docs/cabinet.md § 1. The settings file
as-of: 0e97ce3
body: cabinet
supersedes:
---
[cabinet.md § 1. The settings file](../../../FlipperEngine/docs/cabinet.md#1-the-settings-file)

**The operator's choices live in `settings.json`, not on the command line.** The rule that decides
what goes in it is [architecture.md §7](../../../FlipperEngine/docs/architecture.md#7-configuration): *a fact about the machine
is a constant, a choice made about the machine is configuration.* Switch addresses, the 500 µs
display gap and the 1987 scoring values are facts and are compiled in; these twenty are choices:
