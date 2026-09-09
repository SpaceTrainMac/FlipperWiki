---
title: Every switch, and what closing it does
type: thing
aliases: []
body: game
---
# Every switch, and what closing it does

**All thirty-two, in the order the machine's own table lists them.** *Pays* lands on your score at
once; *advances* changes a count paid when the ball ends; *collects* takes a lit award. Each row
links to the page that explains it. **The rows that do nothing are doing nothing on purpose**: the
matrix belongs to the *1987* MacPinBall System IV chassis rather than to this game, and MAC reused
it for every title it sold ([0184](../../raw/rules/0184-a-macpinball-system-iv-machine-sold-under-multigame.md)).

| Switch | Pays | Advances | Collects | Explained on |
|---|---|---|---|---|
| `M` | **30 000**, when M-A-C is complete | lights or clears the `M` lamp | — | [The M, A and C lanes](../things/m-a-c-lanes.md) |
| `A` | — | lights or clears the `A` lamp; **inert while its own window runs** | when M-A-C is complete, opens a 20 s window on the **upper** `EXTRA BALL` lamp and ends the paying mode | [The M, A and C lanes](../things/m-a-c-lanes.md) |
| `C` | **30 000**, when M-A-C is complete | lights or clears the `C` lamp | — | [The M, A and C lanes](../things/m-a-c-lanes.md) |
| `BUNKER_LEFT` | 100 | starts **multiball** — a second ball is served — if `BALLSENSOR_BALLEJECTOR` has one ready, otherwise the ball is just spat back out | the left ladder's five rungs and marker, if that side's 30 s window is open; a left marker armed with no window running, at any time | [The left bunker](../things/left-bunker.md) |
| `BUNKER_RIGHT` | 100 | — | an **extra ball** when either hole ladder is past rung 2, once a ball; the right ladder's five rungs and marker, if that side's 30 s window is open; a right marker armed with no window running, at any time | [The right bunker](../things/right-bunker.md) |
| `BUMPER_LEFT` | 100 | — | — | [The three pop bumpers](../things/pop-bumpers.md) |
| `BUMPER_RIGHT` | 100 | — | — | [The three pop bumpers](../things/pop-bumpers.md) |
| `BUMPER_MIDDLE` | 100 | — | — | [The three pop bumpers](../things/pop-bumpers.md) |
| `SIDELANE_LEFT_TOP` | — | — | — | [The side lanes](../things/side-lanes.md) |
| `ADVANCE_BONUS_TOP` | 100, first hit of the bank | lights `ADV_BON_TOP`; one bonus if this completes the bank | — | [The four ADVANCE BONUS targets](../things/advance-bonus-targets.md) |
| `ADVANCE_BONUS_ALMOST_TOP` | 100, first hit of the bank | lights `ADV_BON_C_TOP`; one bonus if this completes the bank | — | [The four ADVANCE BONUS targets](../things/advance-bonus-targets.md) |
| `ADVANCE_BONUS_ALMOST_BOTTOM` | 100, first hit of the bank | lights `ADV_BON_C_BOT`; one bonus if this completes the bank | — | [The four ADVANCE BONUS targets](../things/advance-bonus-targets.md) |
| `ADVANCE_BONUS_BOTTOM` | 100, first hit of the bank | lights `ADV_BON_BOT`; one bonus if this completes the bank | — | [The four ADVANCE BONUS targets](../things/advance-bonus-targets.md) |
| `SIDELANE_LEFT_5000` | 5 000 | five bonuses | — | [The 5000 inlanes](../things/inlanes-5000.md) |
| `SIDELANE_RIGHT_5000` | 5 000 | five bonuses | — | [The 5000 inlanes](../things/inlanes-5000.md) |
| `SIDELANE_LEFT_OUT` | 5 000 when `SPECIAL` is lit | — | **SPECIAL** — both lamps go out | [The outlanes](../things/outlanes.md) |
| `SIDELANE_RIGHT_OUT` | 5 000 when `SPECIAL` is lit | — | **SPECIAL** — both lamps go out | [The outlanes](../things/outlanes.md) |
| `SIDELANE_LEFT` | 500 | — | — | [The side lanes](../things/side-lanes.md) |
| `SIDELANE_RIGHT` | 500 | — | — | [The side lanes](../things/side-lanes.md) |
| `SIDEBAR_LEFT_BOTTOM` | — | kicks the ball away | — | [The slingshots](../things/slingshots.md) |
| `SIDEBAR_RIGHT_BOTTOM` | — | kicks the ball away | — | [The slingshots](../things/slingshots.md) |
| `SIDEBAR_RIGHT_TOP` | — | — | — | [The slingshots](../things/slingshots.md) |
| `BALLWITHBALL_LEFT_TWIN` | — | the **left** hole ladder by one rung, or opens/redeems its 30 s window at the 5th/6th hit | the left ladder's five rungs and marker, if that side's window is open | [The two centre captive balls](../things/centre-captive-balls.md) |
| `BALLWITHBALL_RIGHT_TWIN` | — | the **right** hole ladder by one rung, or opens/redeems its 30 s window at the 5th/6th hit | the right ladder's five rungs and marker, if that side's window is open | [The two centre captive balls](../things/centre-captive-balls.md) |
| `BALLWITHBALL_RIGHT_TOP` | **500 000** if `X_BON` is flashing | lights **both** `HOLE BONUS 30000` lamps; lights `X2_BOT` or `X3_BOT` if `X_BON` is flashing | the right `EXTRA BALL` when it is lit (2nd bank completion); the **upper** `EXTRA BALL` inside `A`'s 20 s window | [The right captive ball](../things/right-captive-ball.md) |
| `BALLSENSOR_BALLCACHE` | — | **the drain** — a returning ball reaches the two-ball store here; a pulse is one ball home, a held contact is every ball home and the turn over | — | [The ball store, and the four contacts](../things/ball-store.md) |
| `BALLSENSOR_STARTRAMP` | — | the served ball has **arrived** in the start ramp, ready for the plunger | — | [The ball store, and the four contacts](../things/ball-store.md) |
| `BALLSENSOR_BALLEJECTOR` | — | a ball is **available to serve**; `FCA_1_BALL_OUT` can fire it into the start ramp | — | [The ball store, and the four contacts](../things/ball-store.md) |
| `OUTFIRE` | 1 000 while the left bunker waits for its second ball | the plunger-fired ball has **left the start ramp** into play; opens the drain-protection window | — | [OUTFIRE — the start ramp's exit](../things/outfire.md) |
| `BUTTON_LEFT` | — | rotates the three M-A-C letters left | — | [The flipper buttons](../things/flipper-buttons.md) |
| `BUTTON_RIGHT` | — | rotates the three M-A-C letters right | — | [The flipper buttons](../things/flipper-buttons.md) |
| `BUTTON_START` | — | starts a game and adds players, **at player select and nowhere else**. A game in progress does not read it | — | [The start button](../things/start-button.md) |
