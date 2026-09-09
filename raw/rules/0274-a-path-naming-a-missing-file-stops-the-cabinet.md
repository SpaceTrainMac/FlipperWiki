---
rule: 0274
title: A path naming a file that is not on disk stops the cabinet
source: FlipperEngine/docs/cabinet.md § 3. Sound sets - sounds.json, which file each cue plays
as-of: 0e97ce3
body: cabinet
supersedes:
---
[cabinet.md § 3. Sound sets - sounds.json, which file each cue plays](../../../FlipperEngine/docs/cabinet.md#soundsjson--which-file-each-cue-plays)

**A path naming a file that is not on disk stops the cabinet**, with `E 101` on the glass
([§4](../../../FlipperEngine/docs/cabinet.md#4-troubleshooting)). That is the difference worth knowing: *no entry* is fine, *an entry
pointing at nothing* is a set that was copied half way or a file that was renamed. **Every file in a
list is checked**, so one missing variant out of twelve stops it as surely as a missing single.
