---
rule: 0110
title: Not a playfield lamp
source: FlipperArchitecture/docs/gameplay.md § 13. What the machine shows
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 13. What the machine shows](../../../FlipperArchitecture/docs/gameplay.md#13-what-the-machine-shows)

**Not a playfield lamp, and not idle either: `FDLA_PWM_RED` / `_GREEN` / `_BLUE` read the two bonus
ladders at rest, and [§8](../../../FlipperArchitecture/docs/gameplay.md#8-the-side-lanes-the-sidebars-and-the-bumpers)'s white flashes are a
brief interruption of that** ([hardware.md §5](../../../FlipperArchitecture/docs/hardware.md#5-pwm-backlight)). Each channel is
independently 0–15:

| Channel | Tracks | Formula |
|---|---|---|
| `FDLA_PWM_RED` | the advance bonus, [§5](../../../FlipperArchitecture/docs/gameplay.md#5-the-bonus-count) | that ladder's units digit (0–9) **+ 2 for every `SUPER_BON` lit** (0, 2, 4 or 6) |
| `FDLA_PWM_GREEN` | the left hole bonus, [§6](../../../FlipperArchitecture/docs/gameplay.md#6-the-hole-bonuses-and-the-captive-balls) | that side's rung count (0–5) **+ 5 if `BON_X2_TOP_L` is lit, + 5 more if `BON_X3_TOP_L` is lit** |
| `FDLA_PWM_BLUE` | the right hole bonus, [§6](../../../FlipperArchitecture/docs/gameplay.md#6-the-hole-bonuses-and-the-captive-balls) | that side's rung count (0–5) **+ 5 if `BON_X2_5K_R` is lit, + 5 more if `BON_X3_5K_R` is lit** |
