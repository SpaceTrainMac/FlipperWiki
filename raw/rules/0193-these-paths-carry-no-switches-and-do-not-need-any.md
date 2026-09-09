---
rule: 0193
title: These paths carry no switches, and they do not need any
source: FlipperArchitecture/docs/machine.md § 1.4 Playfield geography
as-of: 0804fe1
body: 1987
supersedes:
---
[machine.md § 1.4 Playfield geography](../../../FlipperArchitecture/docs/machine.md#14-playfield-geography)

These paths carry no switches, and they do not need any: every scoring element has its own switch
ID, so the level is implied by whatever closed. `M` can only be closed by a ball on the upper
playfield. **The two levels are a physical and visual feature, not state the engine has to track** —
if the same elements were laid out flat, the rules would be unchanged.
