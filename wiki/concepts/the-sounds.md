---
title: What the machine says, and when
type: concept
aliases: [the sounds, the sound cues, sfx, LAUNCH_BALL, BALL_IN_GAME, BALL_LOST, HOUSE_BALL_SAVED, GAME_OVER, NEXT_PLAYER, NO_MORE_EXTRABALL, MAIN_BONUS_NEXT_STEP, MAIN_BONUS_ONE_LIGHT, BONUS_COUNT_STEP, BUNKER_LEFT, BUNKER_RIGHT, BUMPER, SIDEBARS_BOTTOM, SPECIAL, TOPLANES_LIGHT_MAC, TOPLANES_SELECT_BONUS, TOPLANES_SUPERBONUS, TOPLANES_XTRABALL, HOLEBONUS_LEFT_NORMAL_HIT, HOLEBONUS_LEFT_DOUBLE, HOLEBONUS_LEFT_TRIPLE, HOLEBONUS_LEFT_BONUS30K_A, HOLEBONUS_LEFT_BONUS30K_B, HOLEBONUS_LEFT_BONUS30K_C, HOLEBONUS_LEFT_BONUS30K_D, HOLEBONUS_LEFT_BONUS30K_E, HOLEBONUS_LEFT_BONUS30K_F, HOLEBONUS_RIGHT_NORMAL_HIT, HOLEBONUS_RIGHT_DOUBLE, HOLEBONUS_RIGHT_TRIPLE, HOLEBONUS_RIGHT_BONUS30K_A, HOLEBONUS_RIGHT_BONUS30K_B, HOLEBONUS_RIGHT_BONUS30K_C, HOLEBONUS_RIGHT_BONUS30K_D, HOLEBONUS_RIGHT_BONUS30K_E, HOLEBONUS_RIGHT_BONUS30K_F, EXTRA_BONUS, SPACE_SHIP_BONUS, SPACE_TRAIN_BONUS]
body: game
---
# What the machine says, and when

**Forty sound cues, and every rule on these pages that says *with its own sound cue* now has one**
([0176](../../raw/rules/0176-settled-and-built.md)). Eleven were added on 2026-09-04 for the rules here — M-A-C's paying lanes, the extra
bonus, and the two the flyer names among them ([0176](../../raw/rules/0176-settled-and-built.md)).

**That the machine speaks at all is 1987's idea.** The sales flyer sells *Info-Speech*, a speaking
announcer, as a System IV feature carried by every machine MAC made — so a talking Space Train is
the chassis doing what it was advertised to do, and the forty cues are this cabinet's answer to it
([0185](../../raw/rules/0185-behaviours-the-flyer-attributes-to-all-macpinball-machines.md)).

**All four sets map the same cues to the same events**, so everything on this page is true of any
of them — an arcade, a blockbuster, an orchestra or a narrator answers the same list ([0277](../../raw/rules/0277-there-are-four-sets-three-generated.md)). See
[sound sets](sound-sets.md).

**[The simulator](../bodies/simulator.md) shows every cue as it is raised, whether or not the
machine is making a noise** — which makes it the place to find out what speaks for a rule without
listening for it ([0242](../../raw/rules/0242-sound-is-off-unless-the-settings-say-so.md)).

**The end-of-ball count is the most obviously cue-shaped thing on the machine**, and it is raised
with every lamp [the count](../moments/end-of-ball.md) puts out — one of the forty is named for a
single rung of it ([0177](../../raw/rules/0177-the-end-of-ball-count-is-the-most-obviously-cue-shaped.md)).

**Until 2026-09-08 every one of those rules described a machine that made no sound** ([0178](../../raw/rules/0178-it-is-designed-and-since-2026-09-08-it-is.md)).

**Forty-three cues and a playlist, and what each cue is *for* is what this page carries** ([0276](../../raw/rules/0276-43-cues-and-a-playlist.md)).
**Which file plays it is not**: that belongs to whichever [sound set](sound-sets.md) is on, and one
set's answer is not another's ([0276](../../raw/rules/0276-43-cues-and-a-playlist.md)). The pages below name the event; the machine names the file
([0276](../../raw/rules/0276-43-cues-and-a-playlist.md)).

**Eleven of the forty are silent on the `rool` set, and that is deliberate** ([0278](../../raw/rules/0278-eleven-rows-are-fixture-only.md)). They were
added on 2026-09-04 and are kept out of that set until a person finds a file for each — its value
is that somebody with taste chose every sound in it, and synthesising one would make it a fourth
generated set wearing the first one's name ([0278](../../raw/rules/0278-eleven-rows-are-fixture-only.md)). **On a cabinet running `rool`, those eleven
events pass in silence** ([0278](../../raw/rules/0278-eleven-rows-are-fixture-only.md)).

**One cue can hold several files, and then the machine picks between them each time it fires**
([0279](../../raw/rules/0279-an-entry-may-name-a-list.md)) — which is [how a bumper stops sounding like the same bumper](sound-sets.md).

**What each cue is for is written down in one place and it is a specification rather than a
description** ([0280](../../raw/rules/0280-what-each-cue-is-for-is-written-down-here.md)). The event a cue answers is what the cue's name and
[the rules](what-the-machine-tracks.md) say it is for — not a readback of the code — and since
2026-09-08 the code has been held to it, one raise per cue, each pinned by a test ([0280](../../raw/rules/0280-what-each-cue-is-for-is-written-down-here.md)). So a
machine that stays quiet at one of these events is wrong about itself ([0280](../../raw/rules/0280-what-each-cue-is-for-is-written-down-here.md)).

## Which cue speaks, and when

**Forty effects and three music cues, in the order the machine's own catalogue lists them.**

### A ball, and a game

| Cue | Speaks when |
|---|---|

| `LAUNCH_BALL` | [a ball is served](../moments/the-serve.md) — the ejector fires and the ball goes to the start ramp ([0281](../../raw/rules/0281-cue-launch-ball.md)) |

| `BALL_IN_GAME` | the served ball reaches the playfield — [`OUTFIRE`](../things/outfire.md) closes ([0282](../../raw/rules/0282-cue-ball-in-game.md)) |

| `BALL_LOST` | **a drain that is not protected** — and in [multiball](../concepts/multiball.md) it fires for a ball lost while the turn continues ([0283](../../raw/rules/0283-cue-ball-lost.md)) |

| `HOUSE_BALL_SAVED` | **a drain inside [the 15-second window](../concepts/drain-protection.md)** — instead of `BALL_LOST`, once a turn ([0284](../../raw/rules/0284-cue-house-ball-saved.md)) |

| `GAME_OVER` | the last ball of the last player has drained ([0285](../../raw/rules/0285-cue-game-over.md)) |

| `NEXT_PLAYER` | [the turn passes](../moments/end-of-turn.md) **to a different player** — a one-player game never hears it ([0286](../../raw/rules/0286-cue-next-player.md)) |

| `NO_MORE_EXTRABALL` | **a drain with [the two-digit field](../things/status-row.md) at zero** — the turn is over ([0287](../../raw/rules/0287-cue-no-more-extraball.md)) |

### The lower playfield

| Cue | Speaks when |
|---|---|

| `MAIN_BONUS_NEXT_STEP` | [the bonus count](../concepts/the-bonus-count.md) advances — **once per advance whatever its size**, so a `5000` inlane's five bonuses is one sound ([0288](../../raw/rules/0288-cue-main-bonus-next-step.md)) |

| `MAIN_BONUS_ONE_LIGHT` | **[the count reaching 39](../concepts/the-bonus-count.md) and stopping** — raised instead of `MAIN_BONUS_NEXT_STEP` ([0289](../../raw/rules/0289-cue-main-bonus-one-light.md)) |

| `BONUS_COUNT_STEP` | **one step of [the end-of-ball count](../moments/end-of-ball.md)** — a lamp goes out, 200 ms later the next ([0290](../../raw/rules/0290-cue-bonus-count-step.md)) |

| `BUNKER_LEFT` | [the left bunker](../things/left-bunker.md) takes the ball — **whatever else that hit does** ([0291](../../raw/rules/0291-cue-bunker-left.md)) |

| `BUNKER_RIGHT` | [the right bunker](../things/right-bunker.md) takes the ball — same rule, the cue is the catch ([0292](../../raw/rules/0292-cue-bunker-right.md)) |

| `BUMPER` | any of [the three pop bumpers](../things/pop-bumpers.md) — **the most-fired cue on the machine by a wide margin** ([0293](../../raw/rules/0293-cue-bumper.md)) |

| `SIDEBARS_BOTTOM` | either of [the two slingshots](../things/slingshots.md) — **the one cue whose event is presentation and nothing else** ([0294](../../raw/rules/0294-cue-sidebars-bottom.md)) |

| `SPECIAL` | **either outlane with [`SPECIAL`](../concepts/special.md) lit** — and `BALL_LOST` gives way to it ([0295](../../raw/rules/0295-cue-special.md)) |

### The upper playfield

| Cue | Speaks when |
|---|---|

| `TOPLANES_LIGHT_MAC` | an [`M`, `A` or `C`](../concepts/m-a-c.md) rollover **toggling** its letter while the word is still being spelled ([0296](../../raw/rules/0296-cue-toplanes-light-mac.md)) |

| `TOPLANES_SELECT_BONUS` | **[the flipper buttons rotating the three letters](../things/flipper-buttons.md)** — the lane change ([0297](../../raw/rules/0297-cue-toplanes-select-bonus.md)) |

| `TOPLANES_SUPERBONUS` | **[M-A-C completing](../concepts/m-a-c.md)**, and `M` or `C` paying its 30 000 while it stands ([0298](../../raw/rules/0298-cue-toplanes-superbonus.md)) |

| `TOPLANES_XTRABALL` | **the upper extra ball collected at [the right captive ball](../things/right-captive-ball.md)** — not at the lane ([0299](../../raw/rules/0299-cue-toplanes-xtraball.md)) |

### The captive balls, and the hole bonus

**The two sides are not symmetric in sound, and that is a repair rather than a design** ([0300](../../raw/rules/0300-the-two-sides-are-not-symmetric.md)).
Each side is [a five-hit build and a timed redemption](../concepts/the-hole-bonus.md), and a
redemption is six things to count out on either side — but the left only got its six lettered cues
on 2026-09-04, where the right had them before ([0300](../../raw/rules/0300-the-two-sides-are-not-symmetric.md)).

**[The third captive ball](../things/right-captive-ball.md) has no cue of its own** ([0301](../../raw/rules/0301-the-third-captive-ball-has-no-cue-of-its-own.md)). It
drives no ladder — it arms both markers, lights the right `EXTRA BALL`, takes the upper one and
takes the extra bonus — so what it raises is **the cue of whatever it just collected** ([0301](../../raw/rules/0301-the-third-captive-ball-has-no-cue-of-its-own.md)).

| Cue | Speaks when |
|---|---|

| `HOLEBONUS_LEFT_NORMAL_HIT` | **rungs 1–5 of [the left ladder](../things/hole-bonus-ladders.md)** — including the fifth, which also opens the window ([0302](../../raw/rules/0302-cue-holebonus-left-normal-hit.md)) |

| `HOLEBONUS_LEFT_DOUBLE` | **the 2nd successful left redemption** — [that side doubles](../concepts/the-multipliers.md) for the rest of the game ([0303](../../raw/rules/0303-cue-holebonus-left-double.md)) |

| `HOLEBONUS_LEFT_TRIPLE` | **the 3rd** — ×3 on the left, and **one of the three lamps [Space Train Bonus](../concepts/flyer-bonuses.md) is waiting for** ([0304](../../raw/rules/0304-cue-holebonus-left-triple.md)) |

| `HOLEBONUS_LEFT_BONUS30K_A` | **the six items of a left redemption, counted out 200 ms apart** — `_A` … `_F`, five rungs and the marker ([0305](../../raw/rules/0305-cue-holebonus-left-bonus30k-a-f.md)) |

| `HOLEBONUS_RIGHT_NORMAL_HIT` | **rungs 1–5 of the right ladder** — [the same 5 000 a rung as the left](../concepts/where-the-sources-are-silent.md) ([0306](../../raw/rules/0306-cue-holebonus-right-normal-hit.md)) |

| `HOLEBONUS_RIGHT_DOUBLE` | the 2nd successful right redemption — ×2 on that side ([0307](../../raw/rules/0307-cue-holebonus-right-double.md)) |

| `HOLEBONUS_RIGHT_TRIPLE` | the 3rd — ×3 on the right, and **the second of [Space Train Bonus](../concepts/flyer-bonuses.md)'s three lamps** ([0308](../../raw/rules/0308-cue-holebonus-right-triple.md)) |

| `HOLEBONUS_RIGHT_BONUS30K_A` | **the six items of a right redemption**, exactly as on the left ([0309](../../raw/rules/0309-cue-holebonus-right-bonus30k-a-f.md)) |

### The two the flyer names, and the one that pays most

**These three are what the 1987 firmware had no word for** ([0310](../../raw/rules/0310-the-three-the-1987-firmware-had-no-word-for.md)). Every cue above was in the
sound player this cabinet ran before the engine existed, and it stopped where the original
behaviour stopped: [Space Ship Bonus and Space Train Bonus](flyer-bonuses.md) were words on a flyer
with no sounds, and [the extra bonus](the-extra-bonus.md) is a rule this project decided ([0310](../../raw/rules/0310-the-three-the-1987-firmware-had-no-word-for.md)).

| Cue | Speaks when |
|---|---|

| `EXTRA_BONUS` | **the right captive ball inside [`X_BON`'s 20-second window](../things/x-bon-lamp.md)** — a flat 500 000 ([0311](../../raw/rules/0311-cue-extra-bonus.md)) |

| `SPACE_SHIP_BONUS` | **`X3_BOT` lighting** — the 50th bank completion, collected. A space-engine warp ([0312](../../raw/rules/0312-cue-space-ship-bonus.md)) |

| `SPACE_TRAIN_BONUS` | **all three ×3 lamps lit** — [the banner](../moments/the-space-train-banner.md), five seconds, and three knocks ([0313](../../raw/rules/0313-cue-space-train-bonus.md)) |

### Five cues that were nearly something else

**Five of the forty stood open, each with two readings its name allowed, and what is kept is which
reading lost** — because a cue settled twice will settle a third way ([0314](../../raw/rules/0314-what-settled-the-five-and-which-reading-lost.md)):

| Cue | Was nearly | Settled as |
|---|---|---|
| `NO_MORE_EXTRABALL` | *earned and refused* | **the last one played off** — nothing on this machine refuses an extra ball |
| `MAIN_BONUS_ONE_LIGHT` | *one lamp still unlit* | **the count reaching 39** — a ladder has exactly one terminal state |
| `TOPLANES_SELECT_BONUS` | *no sound at all* | **the lane change** — the only cue the top lanes offer a player |
| `TOPLANES_SUPERBONUS` | an unbuilt *combination* chain | **M-A-C completing, and `M`/`C` paying** — nothing else is up there |
| the six `BONUS30K` letters | a six-step escalation | **six items counted out** — five rungs and the marker |

*(the table is sound.md §4's, rendered for a player ([0314](../../raw/rules/0314-what-settled-the-five-and-which-reading-lost.md)))*

### Four events that make no sound

**Four things the rules describe have no cue, and they are listed on purpose** — *nobody wrote it
down* is exactly what this catalogue exists to stop ([0315](../../raw/rules/0315-four-events-with-no-cue.md)):

| Event | Why not |
|---|---|
| [the end-of-turn transfer](../moments/end-of-turn.md) | it already sounds like something: 20 ticks of 100 ms, walking the score across |
| **a hole-bonus window opening** at the 5th hit | the 5th hit speaks like the four before it, and six lamps starting to blink is the announcement |
| **a hole-bonus window expiring** uncollected | **the honest gap** — losing 55 000 to a timer is the harshest thing the rules do and the machine says nothing at all |
| [the thunderstrike](the-thunderstrike.md) | it is announced in light: four white flashes of the backlight |

*(the table is sound.md §4's, rendered for a player ([0315](../../raw/rules/0315-four-events-with-no-cue.md)))*
