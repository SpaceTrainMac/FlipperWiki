---
rule: 0104
title: The banner is cut if the ball ends while it stands
source: FlipperArchitecture/docs/gameplay.md § 13. What the machine shows
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 13. What the machine shows](../../../FlipperArchitecture/docs/gameplay.md#13-what-the-machine-shows)

**The banner is cut if the ball ends while it stands.**
[§11](../../../FlipperArchitecture/docs/gameplay.md#11-the-end-of-a-turn-the-transfer)'s transfer is the only other thing that writes these four
displays, and [§10](../../../FlipperArchitecture/docs/gameplay.md#10-the-end-of-a-ball-the-count)'s count buys 1.6 – 4.8 seconds before it, so
the two can only collide if the ball drains within about a second of the achievement. By then the
announcement has been seen and heard, and the count is what pays.
