---
rule: 0221
title: And it is sized on every launch, because VPX will not scale it
source: FlipperVPX/docs/using-the-table.md § 4 — Playing it
as-of: 094e1fe
body: vpx
supersedes:
---
[using-the-table.md § 4 — Playing it](../../../FlipperVPX/docs/using-the-table.md#4--playing-it)

**And it is sized on every launch, because VPX will not scale it.** The playfield does scale: the
table's camera offset is in centimetres and works out as a fraction of the window's *height*
whatever its width, so the picture and the gap it leaves both grow with the display.
`BackglassWidth` and `BackglassHeight` are absolute pixels — VPX reads them as integers and only
clamps them to the window — so a region written for one screen is too small in a widening gap on a
bigger one and sits over the table on a shorter one. `./run_vpx.sh` therefore derives them: **65 % of
the display's height, and the art's own 1024 × 1568 for the width.** On a 1200-tall display that is
509 × 780, which is what this repository ran at all along — the point is not the number, it is that
the number now follows the screen.
