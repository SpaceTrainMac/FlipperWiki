---
rule: 0432
title: Data semantics: zero is the firmware's default, 1 to 127 is milliseconds
source: FlipperArchitecture/docs/hardware.md § 8. Coil cut-off times
as-of: 0804fe1
body: game
supersedes:
---
[hardware.md § 8. Coil cut-off times](../../../FlipperArchitecture/docs/hardware.md#8-coil-cut-off-times)

**Data semantics:**

| Data | Meaning |
|---|---|
| `0` | use the firmware's hardcoded default cut-off time |
| `1` – `127` | override the cut-off time, **in milliseconds** |
