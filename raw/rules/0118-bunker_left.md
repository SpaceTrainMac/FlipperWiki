---
rule: 0118
title: BUNKER_LEFT — what closing it does
source: FlipperArchitecture/docs/gameplay.md § 2. Every switch, and what closing it does
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 2. Every switch, and what closing it does](../../../FlipperArchitecture/docs/gameplay.md#2-every-switch-and-what-closing-it-does)

| Switch | Pays | Advances | Collects |
|---|---|---|---|
| `BUNKER_LEFT` | 100 | starts **multiball** — a second ball is served — if `BALLSENSOR_BALLEJECTOR` has one ready, otherwise the ball is just spat back out | the left ladder's five rungs and marker, if that side's 30 s window is open; a left marker armed with no window running, at any time |
