---
rule: 0427
title: Addresses 232 to 240, and the board de-energises each coil automatically
source: FlipperArchitecture/docs/hardware.md § 6. Coils
as-of: 0804fe1
body: game
supersedes:
---
[hardware.md § 6. Coils](../../../FlipperArchitecture/docs/hardware.md#6-coils)

Addresses **232 – 240**. Data: `0` = off, anything else = fire.
**The board de-energises each coil automatically** — see
[protocol.md §3.2](../../../FlipperArchitecture/docs/protocol.md#32-coil-behaviour--the-safety-mechanism).
Identifiers from `FlipperCoilAddresses`. **All 9 verified.** ✅

| Addr | Schematic | Code identifier | German (sheet) | English |
|---|---|---|---|---|
| 232 | Coil1 | `FCA_1_BALL_OUT` | Kugelauswurf | Ball ejector |
| 233 | Coil2 | `FCA_2_SIDEBAR_LEFT` | Sidebar links | Sidebar left |
| 234 | Coil3 | `FCA_3_SIDEBAR_RIGHT` | Sidebar rechts | Sidebar right |
| 235 | Coil4 | `FCA_4_BUNKER_LEFT` | Bunker links | Bunker left |
| 236 | Coil5 | `FCA_5_BUNKER_RIGHT` | Bunker rechts | Bunker right |
| 237 | Coil6 | `FCA_6_BUMPER_LEFT` | Bumper links | Bumper left |
| 238 | Coil7 | `FCA_7_BUMPER_RIGHT` | Bumper rechts | Bumper right |
| 239 | Coil9 | `FCA_9_BUMPER_CENTER` | Bumper mitte | Bumper centre |
| 240 | CoilK | `FCA_K_KNOCKER` | Knocker | Knocker |
