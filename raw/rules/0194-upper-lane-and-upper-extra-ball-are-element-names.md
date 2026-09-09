---
rule: 0194
title: The card's upper lane and upper extra ball are likewise element names, not a level test
source: FlipperArchitecture/docs/machine.md § 1.4 Playfield geography
as-of: 0804fe1
body: 1987
supersedes:
---
[machine.md § 1.4 Playfield geography](../../../FlipperArchitecture/docs/machine.md#14-playfield-geography)

The card's *"upper lane"* and *"upper extra ball"* are likewise element names, not a level test:
they resolve to specific lamps (`FLA_EXTRA_BALL_TOP`) and specific lanes. Level tracking would only
buy something for presentation — knowing where a ball is during multiball, for sound or display —
which no current rule needs.
