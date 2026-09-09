---
title: Drain protection
type: concept
aliases: [drain protection, the free ball, HOUSE BALL]
body: game
---
# Drain protection

**The first 15 seconds after you launch are covered, and any drain in them gives the ball back**
([0081](../../raw/rules/0081-drain-protection-covers-the-first-15-seconds-configurable.md)). The window is configurable and is measured from the moment the ball leaves the start ramp
([0081](../../raw/rules/0081-drain-protection-covers-the-first-15-seconds-configurable.md)).

**[`HOUSE_BALL`](../things/house-ball-lamp.md) flashes while it is armed.** The playfield prints
`EXTRA BALL` beside that lamp, so a blinking `HOUSE_BALL` reads as *drain now and you still have
your ball* ([0081](../../raw/rules/0081-drain-protection-covers-the-first-15-seconds-configurable.md)).

**The ball comes back on its own — there is no button to press.** Once a game is under way the
start button belongs to player select and the high score table, not to you at the glass ([0082](../../raw/rules/0082-the-ball-comes-back-without-a-press-and.md)).

**The ball it gives back does not count, and nothing is cleared for it.** No count runs, no lamp
goes out, the bonus and both hole ladders stand, and you pick the same ball up where you lost it
([0085](../../raw/rules/0085-the-ball-it-gives-back-does-not-count.md)).

**It covers an outlane as readily as the middle**, and that is a decision rather than a limitation:
the machine can tell them apart and drops the distinction anyway, to guarantee fun and avoid
frustrating the player ([0084](../../raw/rules/0084-it-covers-an-outlane-as-readily-as-the.md)).

**It waits for a ball, not for the drain.** The drained ball needs the length of the trough to roll
back under the ejector, so the serve is triggered by the store reading *available* rather than by the
drain that asked for it ([0083](../../raw/rules/0083-what-the-machine-waits-for-instead-is-a.md)).

**It has a sound of its own, and it replaces the sound of losing a ball.** `HOUSE_BALL_SAVED`
fires where `BALL_LOST` would have, so the machine says which of the two happened before you have
read a single lamp ([what the machine says](the-sounds.md)) ([0284](../../raw/rules/0284-cue-house-ball-saved.md), [0283](../../raw/rules/0283-cue-ball-lost.md)).

**It is spent the first time it saves a drain**, and does not re-arm until your next turn ([0081](../../raw/rules/0081-drain-protection-covers-the-first-15-seconds-configurable.md)).

**On [the VPX table](../bodies/vpx.md) the wait is about 400 ms**, which is how long the trough
takes to put a ball back under the ejector — so a protected drain there feels like the machine
catching the ball rather than like a pause ([0216](../../raw/rules/0216-a-ball-that-drains-in-the-first-fifteen-seconds-is-given-back.md)). **It is also why a machine playing itself serves six balls for three turns** — a two-second ball
is inside the window every time ([0226](../../raw/rules/0226-six-serves-for-a-one-player-game-is-the-machine-being-right.md)). **A ball that stops there and stays is a fault**: until
2026-09-05 the machine waited thirty seconds for a press nobody knew to make, and that behaviour is
gone ([0217](../../raw/rules/0217-a-ball-sitting-in-the-trough-is-a-fault-not-a-rule.md)).
