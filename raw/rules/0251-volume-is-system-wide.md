---
rule: 0251
title: volume is system-wide
source: FlipperEngine/docs/cabinet.md § 1. The settings file
as-of: 0e97ce3
body: cabinet
supersedes:
---
[cabinet.md § 1. The settings file](../../../FlipperEngine/docs/cabinet.md#1-the-settings-file)

**`volume` is system-wide.** `amixer set Master` changes the whole machine's output, and a volume the
engine did not set can be changed out from under it. **That is what every port does**, and not only
the cabinet: this is the volume of *the machine*, and the simulator on a desk and the VPX table are
that machine too, so each of them applies the stored value at start-up.
