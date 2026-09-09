---
rule: 0053
title: A bumper or a slingshot hit also flashes the cabinet's PWM backlight white
source: FlipperArchitecture/docs/gameplay.md § 8. The side lanes, the sidebars and the bumpers
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 8. The side lanes, the sidebars and the bumpers](../../../FlipperArchitecture/docs/gameplay.md#8-the-side-lanes-the-sidebars-and-the-bumpers)

**A bumper or a slingshot hit also flashes the cabinet's PWM backlight white**
([hardware.md §5](../../../FlipperArchitecture/docs/hardware.md#5-pwm-backlight)). `FDLA_PWM_RED`, `_GREEN` and `_BLUE` are each
independently 0–15; a hit drives all three to **15** — full brightness on every channel reads as
white — for the same configurable 300 ms a bumper's own lamp is lit, then restores whatever the
backlight held before the hit ([§13](../../../FlipperArchitecture/docs/gameplay.md#the-cabinet-backlight)). `SIDEBAR_LEFT_BOTTOM` and
`SIDEBAR_RIGHT_BOTTOM` — the two slingshots — trigger the same white flash on their own kick, with
no lamp of their own to go with it; they still score nothing.
