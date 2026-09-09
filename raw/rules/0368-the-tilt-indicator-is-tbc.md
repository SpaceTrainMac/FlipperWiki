---
rule: 0368
title: The TILT indicator
source: FlipperEngine/docs/states/game.md § GameMachine — Tilt is not a host concern
as-of: 0e97ce3
body: game
supersedes:
---
[game.md § GameMachine — Tilt is not a host concern](../../../FlipperEngine/docs/states/game.md#tilt-is-not-a-host-concern)

- **The TILT indicator.** `FDLA_LED_TILT` (address 170) sits in the host-addressable LED block, so
  the host *can* light it — but has no way of knowing when to. Either the firmware drives that lamp
  locally during a tilt, or the host would need to be told. **TBC** against the firmware.
