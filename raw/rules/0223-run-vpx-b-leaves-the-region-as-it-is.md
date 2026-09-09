---
rule: 0223
title: run_vpx.sh -B leaves the region exactly as it is
source: FlipperVPX/docs/using-the-table.md § 4 — Playing it
as-of: 094e1fe
body: vpx
supersedes:
---
[using-the-table.md § 4 — Playing it](../../../FlipperVPX/docs/using-the-table.md#4--playing-it)

**`./run_vpx.sh -B` leaves the region exactly as it is**, for somebody who has placed it by hand.

| On the backbox | |
|---|---|
| **Four player scores** | Six digits each, staggered two by two, the way the real panel is |
| **The status row** | Extra plays, ball in play and credits, bottom left |
| **The match display** | Bottom right, six digits |
| **Sixteen indicator lamps** | The plates around the displays — which player is up, the four x10 multipliers, `EXTRA BALL`, `HIGH SCORE`, `MATCH`, `GAME OVER` and `TILT` |
| **Three round lamps in a strip below the panel** | The cabinet's own RGB backlight, at whatever level the engine is driving it. They fade rather than switch, because the engine drives them as levels |
