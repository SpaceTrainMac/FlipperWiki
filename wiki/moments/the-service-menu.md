---
title: The service menu
type: moment
aliases: [the service menu, SETUP, Setup, the setup menu, the operator menu]
body: cabinet
---
# The service menu

**Hold both flippers for nine seconds while [the cabinet](../bodies/cabinet.md) is in attract mode**
([0252](../../raw/rules/0252-hold-both-flippers-for-nine-seconds.md)). There is no service button — every input in the matrix is a playfield switch or one of
[the three buttons](../things/flipper-buttons.md) — so the way in is a gesture ([0252](../../raw/rules/0252-hold-both-flippers-for-nine-seconds.md)). **A tap
will not do it and one flipper will not do it, and that is deliberate**: both of those happen to a
cabinet all evening ([0252](../../raw/rules/0252-hold-both-flippers-for-nine-seconds.md)).

**After three seconds the light show stops and a joke comes up on the score displays** ([0253](../../raw/rules/0253-after-three-seconds-a-joke-comes-up.md)).
That is the cabinet telling you it is counting: keep holding for the remaining six and the menu
opens, let go and attract mode carries on where it left off. **If you are ever unsure whether the
gesture is working, that is the thing to wait for** ([0253](../../raw/rules/0253-after-three-seconds-a-joke-comes-up.md)).

**There is a second gesture on the same two buttons, and the two cannot be confused** ([0254](../../raw/rules/0254-a-second-gesture-the-right-flipper-alone-starts-the-radio.md)). The
**right flipper alone**, held nine seconds, starts the radio — it reads the same
way, the light show stopping at three seconds with `RADIO` on the glass over a line of scrolling
nonsense ([0254](../../raw/rules/0254-a-second-gesture-the-right-flipper-alone-starts-the-radio.md)). A single-flipper hold only counts while the other button stays up, so reaching
for both with one hand landing first does nothing, and letting go of one hand halfway through the
service gesture does **not** turn the rest of it into a request for the radio ([0254](../../raw/rules/0254-a-second-gesture-the-right-flipper-alone-starts-the-radio.md)). Let go of
both and start again ([0254](../../raw/rules/0254-a-second-gesture-the-right-flipper-alone-starts-the-radio.md)).

## Working it

**Three buttons, and the glass says where you are** ([0255](../../raw/rules/0255-the-value-buttons-repeat-while-held.md)):

| Button | Does |
|---|---|
| start | the next entry, wrapping round |
| right flipper | the current entry's next value |
| left flipper | its previous value |

*(the table is cabinet.md §2's, rendered for a player ([0255](../../raw/rules/0255-the-value-buttons-repeat-while-held.md)))*

**The value buttons repeat while held.** The top pair of [score displays](../things/player-displays.md)
names the entry, the bottom pair shows its value, and [`MATCH`](../things/match-display.md) says
`SETUP` ([0255](../../raw/rules/0255-the-value-buttons-repeat-while-held.md)).

**Seventeen entries in one ring, and start is the only thing that moves between them** — the ring
wraps, so `EXIT` is one press back from `VOLUME` rather than sixteen forward ([0256](../../raw/rules/0256-seventeen-entries-in-one-ring.md)).

| Entry | What it does |
|---|---|
| `VOLUME` | 0–100 in fives. **In force as you step it**, with a short effect at each level so you can hear it |
| `SOUND SET` | `ALL SETS`, then each set found, wrapping. **Needs a restart** — the banner changes to `REBOOT` to say so |
| `SFX MODE` | `RANDOM` or `LOOP` — what a cue naming several files does with them. In force at once |
| `MUSIC` | `ORDER` or `SHUFFLE`. In force at once |
| `RADIO` | which station plays when the cabinet is left alone: `OFF`, then each station, wrapping. `NONE SET` when the file has none |
| `RADIO AFTER` | how long attract waits first — 1, 2, 3, 5, 10, 15, 20, 30, 45 or 60 minutes |
| `CREDITS` | how long the closing titles run, from eleven durations |
| `HIGH SCORES` | **hold** either flipper three seconds to put the table back to `FRITZ` 10000, `ROOL` 9000, `ACE` 8000, `BBB` 7000. A tap does nothing, on purpose |
| `STATISTICS` | **changes nothing** — a flipper steps through what the cabinet has done since it was first switched on |
| `NETWORK` | **changes nothing** — six pages about the machine's network, [the address among them](../bodies/cabinet.md) |
| `RADIO TEST` | a flipper **leaves the menu and starts the radio**, without waiting `RADIO AFTER` out |
| `SWITCH TEST`, `LAMP TEST`, `COIL TEST`, `DISPLAY TEST`, `SOUND TEST` | a flipper leaves the menu and runs that diagnostic. **These are for a machine with its glass off** |
| `EXIT` | either flipper: save and go back to attract mode |

*(the table is cabinet.md §2's, rendered for a player ([0256](../../raw/rules/0256-seventeen-entries-in-one-ring.md)))*

**The last six entries leave the menu rather than change something**, which is why a flipper on one
of them ends the visit — and **everything you adjusted on the way past is saved first**, so a visit
that ends in the coil test does not lose the volume you set ([0257](../../raw/rules/0257-the-last-six-entries-leave-the-menu.md)).

**It saves by itself** — two seconds after you stop adjusting something, and again on the way out.
**Walk away and it closes itself after two minutes, saving first** ([0258](../../raw/rules/0258-the-service-menu-saves-by-itself.md)).
