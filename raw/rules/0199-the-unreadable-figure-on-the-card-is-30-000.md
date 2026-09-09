---
rule: 0199
title: "[?]0.000 is 30 000"
source: FlipperArchitecture/docs/machine.md § 1.5 The instruction cards - Rule card - verbatim
as-of: 0804fe1
body: 1987
supersedes:
---
[machine.md § 1.5 The instruction cards - Rule card - verbatim](../../../FlipperArchitecture/docs/machine.md#rule-card--verbatim)

**`[?]0.000` is 30 000.** The photograph alone cannot separate 3 from 5, but three independent
sources agree: the lamps these rules light are named *"Hole Bonus 30000"* in
`Flipper_Masterplan.xlsx`, the upper target bank is printed `30.000`, and
[`gameHoleBonusLeft.cpp`](../../../FlipperEngine/src/games/gameHoleBonusLeft.cpp) independently awards `30000` for
collecting it. Treat 30 000 as settled unless the machine contradicts it.
