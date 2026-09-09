---
rule: 0234
title: Open the page. The playfield is in the middle and it is where you work
source: FlipperSimulator/docs/using-the-simulator.md § 2. The first five minutes
as-of: 4644649
body: simulator
supersedes:
---
[using-the-simulator.md § 2. The first five minutes](../../../FlipperSimulator/docs/using-the-simulator.md#2-the-first-five-minutes)

**Open the page. The playfield is in the middle and it is where you work.**

1. **Press start.** Click the start button along the bottom of the picture, or press `s`. The
   attract mode ends and the glass asks how many are playing - `1 PLAYER`. The state panel on the
   right moves from *intro* to *player select*.
2. **Press start again.** The game begins: the eject coil at the foot of the shooter lane flares,
   because the engine has just served the first ball into the lane. Nothing else happens, because
   the ball is not on the playfield yet, and there is no ball.
3. **Put it on the playfield.** Press `o` — *Out Fire*, the switch at the top of the shooter lane.
   The engine counts the ball as in play from here, and the fifteen-second drain protection starts.
4. **Hit something.** `q`, `w` and `e` are the three pop bumpers. Watch the score displays on the
   left redraw from the bytes the engine actually put on the wire, and the coils flare on the
   playfield.
5. **Stage the next ball.** Press `1` — *ball at the eject coil*. It is a **toggle**: it stays
   closed, because that is what a ball resting on a switch does. Nothing fires yet; the engine only
   wants to know the store has one.
6. **Drain it.** Press `3` — *ball in the store*, a toggle too. Inside fifteen seconds of `o` the
   drain is protected: nothing is counted, and the eject coil flares again at once, because `1`
   says a ball is staged - since 2026-09-05 a saved ball comes back with no press. Press `3` again
   to open the store, `o` to put the served ball in play, wait the fifteen seconds out, and the
   next `3` ends the turn: the ball counter on the status row goes down, and with `1` still closed
   the next ball is served straight away.
