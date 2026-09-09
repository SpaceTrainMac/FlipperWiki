---
rule: 0236
title: Nothing in the simulator ever moves a switch by itself
source: FlipperSimulator/docs/using-the-simulator.md § 2. The first five minutes
as-of: 4644649
body: simulator
supersedes:
---
[using-the-simulator.md § 2. The first five minutes](../../../FlipperSimulator/docs/using-the-simulator.md#2-the-first-five-minutes)

**Nothing in the simulator ever moves a switch by itself.** A coil firing does not empty the bunker
whose switch you closed; that would be a ball moving, and there is no ball. **A bunker that looks
stuck is a bunker you left closed.** And a ball you staged with `1` stays staged until you open it:
every drain will be answered with a serve for as long as it is closed.
