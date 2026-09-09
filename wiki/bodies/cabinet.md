---
title: The cabinet
type: body
aliases: [the cabinet, the real machine, the machine in the room, the Pi, the operator]
body: cabinet
---
# The cabinet

**The machine itself: a 1987 playfield with a Raspberry Pi where the relay logic used to be** —
and the only body that can be left alone in a room and found still doing something. Everything this
wiki says about the game is true here; what is different is that somebody owns it and can change
things about it.

## What can be changed at all

**There is a line between a fact about this machine and a choice made about it, and it decides
what is adjustable** ([0244](../../raw/rules/0244-the-operators-choices-live-in-settings-json.md)). A switch address, the 500 µs gap between display writes and the
[1987 scoring values](1987.md) are facts and are built in; twenty things are choices and live in a
settings file ([0244](../../raw/rules/0244-the-operators-choices-live-in-settings-json.md)). **Nothing about how the game scores can be turned into a setting** — that
is what makes this wiki's numbers safe to quote on any body ([0244](../../raw/rules/0244-the-operators-choices-live-in-settings-json.md)).

**Changing one no longer means an ssh session: the cabinet serves a page that edits the file, shows
what the engine made of it and restarts** ([0245](../../raw/rules/0245-editing-it-no-longer-means-an-ssh-session.md)). **The address is on the glass**, in the service
menu's `NETWORK` page — so the way to find the machine on a network is to ask the machine ([0245](../../raw/rules/0245-editing-it-no-longer-means-an-ssh-session.md)).

**Seven of them can be set at the machine itself, with no keyboard and no ssh** — the volume, which
sound set plays, how a cue with several files picks one, how the jukebox picks, which radio station,
how long the machine waits before starting the radio, and how long the closing titles run ([0246](../../raw/rules/0246-seven-of-the-eighteen-are-editable-at-the-machine.md)).
The service menu writes them straight back ([0246](../../raw/rules/0246-seven-of-the-eighteen-are-editable-at-the-machine.md)). **The radio has a second way in: the right
flipper steps stations while the radio is playing**, and every press is saved at once ([0246](../../raw/rules/0246-seven-of-the-eighteen-are-editable-at-the-machine.md)).

**And the volume of the radio has a way in of its own: hold the left flipper while it is playing
and the level climbs**, taking effect and saving itself when you let go ([0247](../../raw/rules/0247-hold-the-left-flipper-while-the-radio-is-playing.md)). It is done this
way because **a volume is judged by ear and the service menu is silent** ([0247](../../raw/rules/0247-hold-the-left-flipper-while-the-radio-is-playing.md)).
