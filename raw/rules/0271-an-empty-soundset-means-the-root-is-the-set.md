---
rule: 0271
title: An empty soundSet means the root itself is the set
source: FlipperEngine/docs/cabinet.md § 3. Sound sets - Where the sets live, and which one plays
as-of: 0e97ce3
body: cabinet
supersedes:
---
[cabinet.md § 3. Sound sets - Where the sets live, and which one plays](../../../FlipperEngine/docs/cabinet.md#where-the-sets-live-and-which-one-plays)

**An empty `soundSet` means the root itself is the set.** A cabinet with only one set can put that
set's `sounds.json` and folders straight into `soundRoot` and leave the setting empty. `NONE SET` in
the menu means no directory under the root holds a `sounds.json` — usually the root pointing
somewhere else than you think.
