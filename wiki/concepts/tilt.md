---
title: Tilt
type: concept
aliases: [tilt, TILT]
body: game
---
# Tilt

**Tilt is the cabinet's own business, and the game never hears about one.** The cabinet kills its own
outputs until the balls have drained and never tells the software, which sees an ordinary drain and
counts the bonus for it ([0090](../../raw/rules/0090-tilt-is-the-machines-own-business-and-nothing.md)).

**So a tilt does not void the ball's bonus** — none of the machine's 32 switch inputs is a tilt bob,
so voiding it is not one of the behaviours available ([0090](../../raw/rules/0090-tilt-is-the-machines-own-business-and-nothing.md)).

**What you lose to a tilt is every output the cabinet has just switched off**, which is punishment
enough ([0090](../../raw/rules/0090-tilt-is-the-machines-own-business-and-nothing.md)).

**On [the VPX table](../bodies/vpx.md) the tilt key is VPX's own** — it is not a switch on this
machine and the game is not told, which is the same arrangement the cabinet has ([0219](../../raw/rules/0219-the-other-keys-vpx-offers-reach-nothing.md)). **VPX handles the
whole of a nudge itself and the engine sees an ordinary drain**, so on that body the `TILT` plate
is drawn and can never light ([0229](../../raw/rules/0229-your-nudge-does-not-talk-to-the-game.md)).

**It works the same way [the flippers](../things/flipper-buttons.md) do: in hardware, bypassing the
game entirely** ([0367](../../raw/rules/0367-tilt-works-in-hardware-bypassing-the-game.md)). The machine kills its own outputs and keeps them off until the balls have
left the playfield; the game is not consulted and cannot veto it — **which is the right design,
since a tilt has to work when the computer is not healthy** ([0367](../../raw/rules/0367-tilt-works-in-hardware-bypassing-the-game.md)). What the game sees is the
aftermath: the ball drains, the drain contact fires, and the ball ends through the ordinary path
([0367](../../raw/rules/0367-tilt-works-in-hardware-bypassing-the-game.md)).

TBC — **whether the `TILT` plate on the backbox ever lights on the cabinet is not settled**
([0368](../../raw/rules/0368-the-tilt-indicator-is-tbc.md)). It is in the host-addressable range, so the machine *can* light it and has no way of
knowing when to; either the cabinet's own wiring lights it locally during a tilt, or the game would
have to be told ([0368](../../raw/rules/0368-the-tilt-indicator-is-tbc.md)). Only the cabinet can answer it ([0368](../../raw/rules/0368-the-tilt-indicator-is-tbc.md)). **On
[the VPX table](../bodies/vpx.md) it is drawn and can never light**
([0229](../../raw/rules/0229-your-nudge-does-not-talk-to-the-game.md)).

**Real machines usually void the ball's bonus on a tilt, and this one does not** ([0369](../../raw/rules/0369-tilt-and-bonus-forfeit.md)). The
state document raises it as an open question and points at the rules to settle it; **the rules
have** — the bonus is counted for a tilted ball like any other, because nothing in the matrix is a
tilt bob ([0090](../../raw/rules/0090-tilt-is-the-machines-own-business-and-nothing.md)) ([0369](../../raw/rules/0369-tilt-and-bonus-forfeit.md)).
