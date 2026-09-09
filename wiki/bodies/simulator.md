---
title: The browser simulator
type: body
aliases: [the simulator, the browser simulator, the page, mcp's page, the instrument]
body: simulator
---
# The browser simulator

**The third body, and the only one with no ball in it** ([0234](../../raw/rules/0234-open-the-page-the-playfield-is-where-you-work.md)). The playfield is a picture in the
middle of a web page, every switch is a key or a click, and the engine behind it is the same engine
the cabinet runs — so everything this wiki says about the game is true here, except that nothing
moves unless you move it.

## Getting a ball into play

**Six presses, and they are the machine's own sequence rather than the page's** ([0234](../../raw/rules/0234-open-the-page-the-playfield-is-where-you-work.md)):

| | Do | What happens |
|---|---|---|
| 1 | press start, or `s` | attract ends and the glass asks `1 PLAYER` |
| 2 | press start again | the eject coil flares — [a ball has been served into the ramp](../moments/the-serve.md) |
| 3 | press `o` — [`OUTFIRE`](../things/outfire.md) | the ball counts as in play, and [drain protection](../concepts/drain-protection.md)'s fifteen seconds start |
| 4 | press `q`, `w`, `e` | [the three bumpers](../things/pop-bumpers.md); the displays redraw from the bytes the engine put on the wire |
| 5 | press `1` — ball at the eject coil | a **toggle**: it stays closed, because that is what a ball resting on a switch does |
| 6 | press `3` — ball in the store | the drain. Inside fifteen seconds of `o` it is protected and the coil flares again at once |

*(the six steps are using-the-simulator.md §2's, rendered for a player ([0234](../../raw/rules/0234-open-the-page-the-playfield-is-where-you-work.md)))*

**Step 6 is the one that teaches the machine.** Press `3` again to open the store, `o` to put the
served ball in play, wait the fifteen seconds out, and the next `3` ends the turn — the ball
counter on [the status row](../things/status-row.md) goes down, and with `1` still closed the next
ball is served straight away ([0234](../../raw/rules/0234-open-the-page-the-playfield-is-where-you-work.md)).

**The start button does nothing during a game here either** — it belongs to player select and to
the high score table, and between the two the engine serves every ball itself ([0235](../../raw/rules/0235-the-start-button-does-nothing-during-a-game.md)).

**Nothing here ever moves a switch by itself** ([0236](../../raw/rules/0236-nothing-ever-moves-a-switch-by-itself.md)). A coil firing does not empty the bunker
whose switch you closed — that would be a ball moving, and there is no ball. So **a bunker that
looks stuck is a bunker you left closed**, and a ball you staged with `1` stays staged until you
open it: every drain is answered with a serve for as long as it is ([0236](../../raw/rules/0236-nothing-ever-moves-a-switch-by-itself.md)).

## Reading the picture

**Three kinds of control, drawn differently because they behave differently** ([0237](../../raw/rules/0237-the-three-kinds-of-control.md)):

| Kind | How many | Behaves like |
|---|---|---|
| **momentary** | most | one click closes and reopens — a target, a rollover, a slingshot |
| **toggle**, with a blue ring | five | [both bunkers](../things/left-bunker.md) and the three ball-rest sensors: click to close, click again to open, because a ball can hold them shut indefinitely |
| **cabinet button**, drawn apart | three | [start](../things/start-button.md) and [the two flipper buttons](../things/flipper-buttons.md) — **held, not tapped**: they close on the way down and open on the way up |

*(the table is using-the-simulator.md §2's, rendered for a player ([0237](../../raw/rules/0237-the-three-kinds-of-control.md)))*

**That last row is what makes the service menu reachable** ([0238](../../raw/rules/0238-cabinet-buttons-are-held-not-tapped.md)): both flippers held together
for nine seconds opens `Setup`, and a button that released itself a millisecond later could never
get there — hold `ArrowLeft` and `ArrowRight` together and count ([0238](../../raw/rules/0238-cabinet-buttons-are-held-not-tapped.md)).

**A lamp is a level. On is on** ([0239](../../raw/rules/0239-a-lamp-is-a-level.md)).
