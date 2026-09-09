---
rule: 0225
title: spacetrain-autoplay plays a whole game with nobody at the keyboard
source: FlipperVPX/docs/using-the-table.md § 4 — Playing it - Letting it play itself
as-of: 094e1fe
body: vpx
supersedes:
---
[using-the-table.md § 4 — Playing it - Letting it play itself](../../../FlipperVPX/docs/using-the-table.md#letting-it-play-itself)

**`spacetrain-autoplay` plays a whole game with nobody at the keyboard**, and it needs no VPX at all
— it drives the same engine through the switch matrix directly, so it runs on any machine that can
build this repository.

```bash
./build/spacetrain-autoplay          # one player
./build/spacetrain-autoplay -p 4     # four
./build/spacetrain-autoplay -p 2 -q  # only the closing report
```

It presses START, answers the ejector coil with the switch chain a ball would close, keeps the ball
alive for two seconds, drains it, and types initials at the end. A run takes **29 seconds at one
player and about 110 at four**, exits `0` when the game finished and every invariant held, and
prints the state path it took:

```
  states    intro -> player select -> play -> highscore -> show highscore
  serves    6   drains 6   double 0
```
