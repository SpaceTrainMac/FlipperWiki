---
rule: 0024
title: The ladder rolls its tens over as it fills
source: FlipperArchitecture/docs/gameplay.md § 5. The bonus count
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 5. The bonus count](../../../FlipperArchitecture/docs/gameplay.md#5-the-bonus-count)

**The ladder rolls its tens over as it fills.** A bank completion always steps it by exactly one,
but a `5000` inlane can jump it by five in one hit and cross a decade boundary: reaching a multiple
of ten fills what is left of the old decade, blanks all nine at once, lights the Super Bonus lamp
for the decade just completed, and refills to the new units digit — so the playfield always reads as
the count.
