---
rule: 0256
title: Seventeen entries in one ring
source: FlipperEngine/docs/cabinet.md § 2. The service menu
as-of: 0e97ce3
body: cabinet
supersedes:
---
[cabinet.md § 2. The service menu](../../../FlipperEngine/docs/cabinet.md#2-the-service-menu)

**Seventeen entries in one ring**, and the start button is the only thing that moves between them. The
ring wraps, so `EXIT` is one press back from `VOLUME` rather than sixteen forward.

| Entry | What it does |
|---|---|
| `VOLUME` | 0–100 in fives. **In force as you step it**, and it plays a short effect at each new level so you can hear it |
| `SOUND SET` | `ALL SETS`, then each set found under `soundRoot`, wrapping. **Needs a restart** — the banner changes to `REBOOT` to say so. `ALL SETS` writes `"*"` and pools every set into one cabinet; there is one mixer and no ducking, so the sets are heard at whatever levels their authors chose |
| `SFX MODE` | `RANDOM` or `LOOP`: what a cue that names several files does with them. In force at once, unlike the row above it |
| `MUSIC` | `ORDER` or `SHUFFLE`. In force at once |
| `RADIO` | which station plays when the cabinet is left alone: `OFF`, then each station in `radioStations`, wrapping. `NONE SET` when you have not put any in the file yet |
| `RADIO AFTER` | how long attract mode waits before the radio starts — 1, 2, 3, 5, 10, 15, 20, 30, 45 or 60 minutes |
| `CREDITS` | how long the closing titles run, from a list of eleven durations |
| `HIGH SCORES` | **hold** either flipper for three seconds to put the table back to its four defaults — `FRITZ` 10000, `ROOL` 9000, `ACE` 8000, `BBB` 7000. A tap does nothing on purpose; this is the one thing here you cannot undo with the other flipper. It writes `highscores.csv` immediately, not `settings.json` |
| `STATISTICS` | **changes nothing** — a flipper steps through what the cabinet has done since it was first switched on: games, player-games, balls served, total points, ball travel, time in play, hours on, extra and free balls, multiballs, tilts, draws won, places taken in the table, best ball, longest ball, and the date it started counting — then one page per radio station that has actually been listened to. **The top row says which statistic rather than `STATISTICS`**, because `TOTAL POINTS` is twelve characters on its own; `MATCH` still says `SETUP`, which is what tells you where you are. **There is no reset**: an odometer that can be wound back is not one, and the way to start again is `rm statistics.json` over ssh |
| `NETWORK` | **changes nothing** — a flipper steps through six pages telling you what the cabinet knows about its network: the interface, the SSID, signal strength, the address, whether the internet is reachable, and what the radio last did |
| `RADIO TEST` | a flipper **leaves the menu and starts the radio**, without waiting out `RADIO AFTER`. Both flippers held bring you back here, so this and `NETWORK` are the pair to use when a station will not play |
| `SWITCH TEST`, `LAMP TEST`, `COIL TEST`, `DISPLAY TEST`, `SOUND TEST` | a flipper leaves the menu and runs that diagnostic. **These are for a machine with its glass off** — what each one shows is [states/hardware-tests.md](../../../FlipperEngine/docs/states/hardware-tests.md). `BUTTON_START` ends any of them, back to attract mode |
| `EXIT` | either flipper: save and go back to attract mode |
