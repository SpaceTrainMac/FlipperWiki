---
title: What the machine says, and when
type: concept
aliases: [the sounds, the sound cues, sfx, LAUNCH_BALL, BALL_IN_GAME, BALL_LOST, HOUSE_BALL_SAVED, GAME_OVER, NEXT_PLAYER, NO_MORE_EXTRABALL, MAIN_BONUS_NEXT_STEP, MAIN_BONUS_ONE_LIGHT, BONUS_COUNT_STEP, BUNKER_LEFT, BUNKER_RIGHT, BUMPER, SIDEBARS_BOTTOM]
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
