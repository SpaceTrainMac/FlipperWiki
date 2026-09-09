---
rule: 0222
title: It is the display VPX will open on, in its logical size, that counts
source: FlipperVPX/docs/using-the-table.md § 4 — Playing it
as-of: 094e1fe
body: vpx
supersedes:
---
[using-the-table.md § 4 — Playing it](../../../FlipperVPX/docs/using-the-table.md#4--playing-it)

**It is the display VPX will open on, in its *logical* size, that counts — and the desktop's idea
of the main screen is not VPX's.** VPX takes `[Player] PlayfieldDisplay` and otherwise SDL's primary
display; on a laptop beside a 4K screen GNOME calls the panel primary and SDL calls the screen
primary. So the launcher asks first through `tools/vpx_display.py`, which loads the `libSDL3` VPX
was built against and asks it the question VPX asks, and prints the size VPX will see — logical
pixels, so a 3072 × 1920 panel at 160 % answers 1920 × 1200. Only where that cannot answer does it
fall back to GNOME's own reading and then to `xrandr`, which reports the panel and would be 60 % too
big; on a desktop that answers none of the three, the launcher says so in one line and leaves the
file alone. The Mac is that desktop today: the dylib's place inside the bundle is not known from
here.
