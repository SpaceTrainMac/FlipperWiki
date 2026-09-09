---
rule: 0420
title: The reading matter is only half of it — the cabinet is lit as well
source: FlipperEngine/docs/states/credits.md § CreditsMachine — The light show
as-of: 0e97ce3
body: game
supersedes:
---
[credits.md § CreditsMachine — The light show](../../../FlipperEngine/docs/states/credits.md#the-light-show)

The reading matter is only half of it — the cabinet is lit as well, and the two halves are
deliberately unalike:

| | What it does | Why that shape |
|---|---|---|
| the 48 playfield lamps ([hardware.md §4](../../../FlipperArchitecture/docs/hardware.md#4-playfield-lamps)) | one random lamp on and another random lamp off, every 50 ms cycle | no pattern to spot, so it never looks like a sequence that has got stuck |
| the RGB backlight ([hardware.md §5](../../../FlipperArchitecture/docs/hardware.md#5-pwm-backlight)) | three sine waves, wavelengths 1 : 2 : 4 | the slowest thing on the cabinet, against the fastest |
