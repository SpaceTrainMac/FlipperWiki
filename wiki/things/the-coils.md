---
title: The nine coils
type: thing
aliases: [the coils, the solenoids, FCA_1_BALL_OUT, FCA_2_SIDEBAR_LEFT, FCA_3_SIDEBAR_RIGHT, FCA_4_BUNKER_LEFT, FCA_5_BUNKER_RIGHT, FCA_6_BUMPER_LEFT, FCA_7_BUMPER_RIGHT, FCA_9_BUMPER_CENTER, FCA_K_KNOCKER, the ball ejector, the kickers]
body: game
---
# The nine coils

**Nine coils are everything this machine can do to a ball, and you hear all of them** ([0427](../../raw/rules/0427-the-nine-coils.md)):

| Coil | What it is |
|---|---|
| `FCA_1_BALL_OUT` | [the ball ejector](../things/ball-store.md) — the serve |
| `FCA_2_SIDEBAR_LEFT`, `FCA_3_SIDEBAR_RIGHT` | [the two slingshots](slingshots.md) |
| `FCA_4_BUNKER_LEFT`, `FCA_5_BUNKER_RIGHT` | [the two saucers](left-bunker.md) kicking the ball back out |
| `FCA_6_BUMPER_LEFT`, `FCA_7_BUMPER_RIGHT`, `FCA_9_BUMPER_CENTER` | [the three pop bumpers](pop-bumpers.md) |
| `FCA_K_KNOCKER` | [the knocker](knocker.md) |

*(the table is hardware.md §6's, rendered for a player ([0427](../../raw/rules/0427-the-nine-coils.md)))*

**Nothing has to switch one off** — the board de-energises each coil by itself, which is what stops
a stuck output from burning a coil out ([0427](../../raw/rules/0427-the-nine-coils.md)).

**There is no Coil8** — the schematic's numbering skips it and the code keeps the gap, which is why
the third bumper is `FCA_9_` and not `FCA_8_` ([0428](../../raw/rules/0428-there-is-no-coil8.md)).

**The flipper coils are not among the nine** — they are not driven by the game at all: **the
buttons drive them directly in hardware, and the game's only say is one relay that gates the whole
circuit** ([0429](../../raw/rules/0429-the-flipper-coils-are-not-in-this-list.md)). That is what [0218](../../raw/rules/0218-your-flipper-keys-are-vpxs-own.md)
means when it says the flippers go dead rather than sluggish ([0429](../../raw/rules/0429-the-flipper-coils-are-not-in-this-list.md)).

**The machine has five relay addresses and one wired relay** — `FRA_NO_PADDLE_MODE`, which
disables the flippers. The other four are not connected to anything ([0430](../../raw/rules/0430-only-one-relay-is-wired.md)).

**Each of the nine has a cut-off time of its own, on an address beside it** — so how long a coil
fires can be set per coil rather than for all of them ([0431](../../raw/rules/0431-one-cut-off-time-per-coil.md)).

**A cut-off time is a number of milliseconds, and zero means *use the firmware's own default***
— 1 to 127 overrides it ([0432](../../raw/rules/0432-a-cut-off-time-is-milliseconds-or-the-default.md)). **So a coil nobody has tuned is not a coil with no cut-off**:
zero is a choice to let the board decide ([0432](../../raw/rules/0432-a-cut-off-time-is-milliseconds-or-the-default.md)).
