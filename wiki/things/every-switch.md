---
title: Every switch, and what closing it does
type: thing
aliases: []
body: game
---
# Every switch, and what closing it does

**All thirty-two, in the order the machine's own table lists them.** *Pays* lands on your score at
once; *advances* changes a count paid when the ball ends; *collects* takes a lit award. Each row
links to the page that explains it.

| Switch | Pays | Advances | Collects | Explained on |
|---|---|---|---|---|
| `M` | **30 000**, when M-A-C is complete | lights or clears the `M` lamp | — | [m a c lanes](../things/m-a-c-lanes.md) |
| `A` | — | lights or clears the `A` lamp; **inert while its own window runs** | when M-A-C is complete, opens a 20 s window on the **upper** `EXTRA BALL` lamp and ends the paying mode (§3) | [m a c lanes](../things/m-a-c-lanes.md) |
| `C` | **30 000**, when M-A-C is complete | lights or clears the `C` lamp | — | [m a c lanes](../things/m-a-c-lanes.md) |
| `BUNKER_LEFT` | 100 | starts **multiball** — a second ball is served — if `BALLSENSOR_BALLEJECTOR` has one ready, otherwise the ball is just spat back out | the left ladder's five rungs and marker, if that side's 30 s window is open; a left marker armed with no window running, at any time | [left bunker](../things/left-bunker.md) |
| `BUNKER_RIGHT` | 100 | — | an **extra ball** when either hole ladder is past rung 2, once a ball; the right ladder's five rungs and marker, if that side's 30 s window is open; a right marker armed with no window running, at any time | [right bunker](../things/right-bunker.md) |
| `BUMPER_LEFT` | 100 | — | — | [pop bumpers](../things/pop-bumpers.md) |
| `BUMPER_RIGHT` | 100 | — | — | [pop bumpers](../things/pop-bumpers.md) |
| `BUMPER_MIDDLE` | 100 | — | — | [pop bumpers](../things/pop-bumpers.md) |
| `SIDELANE_LEFT_TOP` | — | — | — | [side lanes](../things/side-lanes.md) |
| `ADVANCE_BONUS_TOP` | 100, first hit of the bank | lights `ADV_BON_TOP`; one bonus if this completes the bank | — | [advance bonus targets](../things/advance-bonus-targets.md) |
| `ADVANCE_BONUS_ALMOST_TOP` | 100, first hit of the bank | lights `ADV_BON_C_TOP`; one bonus if this completes the bank | — | [advance bonus targets](../things/advance-bonus-targets.md) |
| `ADVANCE_BONUS_ALMOST_BOTTOM` | 100, first hit of the bank | lights `ADV_BON_C_BOT`; one bonus if this completes the bank | — | [advance bonus targets](../things/advance-bonus-targets.md) |
| `ADVANCE_BONUS_BOTTOM` | 100, first hit of the bank | lights `ADV_BON_BOT`; one bonus if this completes the bank | — | [advance bonus targets](../things/advance-bonus-targets.md) |
| `SIDELANE_LEFT_5000` | 5 000 | five bonuses | — | [inlanes 5000](../things/inlanes-5000.md) |
| `SIDELANE_RIGHT_5000` | 5 000 | five bonuses | — | [inlanes 5000](../things/inlanes-5000.md) |
| `SIDELANE_LEFT_OUT` | 5 000 when `SPECIAL` is lit | — | **SPECIAL** — both lamps go out | [outlanes](../things/outlanes.md) |
| `SIDELANE_RIGHT_OUT` | 5 000 when `SPECIAL` is lit | — | **SPECIAL** — both lamps go out | [outlanes](../things/outlanes.md) |
| `SIDELANE_LEFT` | 500 | — | — | [side lanes](../things/side-lanes.md) |
| `SIDELANE_RIGHT` | 500 | — | — | [side lanes](../things/side-lanes.md) |
| `SIDEBAR_LEFT_BOTTOM` | — | kicks the ball away | — | [slingshots](../things/slingshots.md) |
| `SIDEBAR_RIGHT_BOTTOM` | — | kicks the ball away | — | [slingshots](../things/slingshots.md) |
| `SIDEBAR_RIGHT_TOP` | — | — | — | [slingshots](../things/slingshots.md) |
| `BALLWITHBALL_LEFT_TWIN` | — | the **left** hole ladder by one rung, or opens/redeems its 30 s window at the 5th/6th hit | the left ladder's five rungs and marker, if that side's window is open | [centre captive balls](../things/centre-captive-balls.md) |
| `BALLWITHBALL_RIGHT_TWIN` | — | the **right** hole ladder by one rung, or opens/redeems its 30 s window at the 5th/6th hit | the right ladder's five rungs and marker, if that side's window is open | [centre captive balls](../things/centre-captive-balls.md) |
| `BALLWITHBALL_RIGHT_TOP` | **500 000** if `X_BON` is flashing | lights **both** `HOLE BONUS 30000` lamps; lights `X2_BOT` or `X3_BOT` if `X_BON` is flashing | the right `EXTRA BALL` when it is lit (2nd bank completion); the **upper** `EXTRA BALL` inside `A`'s 20 s window | [right captive ball](../things/right-captive-ball.md) |
| `BALLSENSOR_BALLCACHE` | — | **the drain** — a returning ball reaches the two-ball store here; a pulse is one ball home, a held contact is every ball home and the turn over (§12) | — | [ball store](../things/ball-store.md) |
