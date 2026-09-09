---
rule: 0248
title: No settings file is a first boot, not a fault
source: FlipperEngine/docs/cabinet.md § 1. The settings file
as-of: 0e97ce3
body: cabinet
supersedes:
---
[cabinet.md § 1. The settings file](../../../FlipperEngine/docs/cabinet.md#1-the-settings-file)

- **No settings file is a first boot, not a fault.** Every value takes its default and start-up says
  `settings.json  (not found - defaults)`. A cabinet with one sound set in `./` runs with no settings
  file at all.
