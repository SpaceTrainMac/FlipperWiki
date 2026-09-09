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
