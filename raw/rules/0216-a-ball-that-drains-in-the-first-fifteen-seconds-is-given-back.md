---
rule: 0216
title: A ball that drains in the first fifteen seconds is given back, and it comes back on its own
source: FlipperVPX/docs/using-the-table.md § 4 — Playing it
as-of: 094e1fe
body: vpx
supersedes:
---
[using-the-table.md § 4 — Playing it](../../../FlipperVPX/docs/using-the-table.md#4--playing-it)

**A ball that drains in the first fifteen seconds is given back, and it comes back on its own.**
`GameFreeBall` arms drain protection when the ball passes out-fire and holds it open for **15 s**,
once per turn; a drain inside that window does not end the turn, and the ejector fires again as soon
as the trough has put a ball back under it — about **400 ms** on this table. `HOUSE_BALL`, lamp
**228**, blinks while the protection is armed.
