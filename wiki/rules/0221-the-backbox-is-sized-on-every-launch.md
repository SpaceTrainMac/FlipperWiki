---
title: The backbox region is derived at launch, because VPX treats it as absolute pixels
type: rule
aliases: []
body: vpx
---
# Rule 0221 — And it is sized on every launch

**At the glass: the backbox is the right size on your screen because it was measured for your
screen, seconds ago** ([0221](../../raw/rules/0221-the-backbox-is-sized-on-every-launch.md)). VPX reads the region as absolute pixels and never scales it, so the
launcher recomputes it from the display's height each time — 65 % of it, at the artwork's own
proportions ([0221](../../raw/rules/0221-the-backbox-is-sized-on-every-launch.md)). Pages: [the Visual Pinball table](../bodies/vpx.md).
