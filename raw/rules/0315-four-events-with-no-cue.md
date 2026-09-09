---
rule: 0315
title: Four events the rules describe still have no cue
source: FlipperEngine/docs/sound.md § 4. The catalogue - Four events with no cue
as-of: 0e97ce3
body: game
supersedes:
---
[sound.md § 4. The catalogue - Four events with no cue](../../../FlipperEngine/docs/sound.md#four-events-with-no-cue-and-why-that-is-not-eleven-more)

**Eleven cues were added on 2026-09-04 and four events the rules describe still have none.** They
are listed because *nobody wrote it down* is what this section exists to stop happening twice:

| Event | Where | Why not |
|---|---|---|
| **the end-of-turn transfer** — 20 ticks of 100 ms walking the turn score across | [gameplay.md §11](../../../FlipperArchitecture/docs/gameplay.md#11-the-end-of-a-turn-the-transfer) | it already has a sound in the only sense that matters — the knocker, at the tick the total passes the record — and a cue under a 2-second animation that follows 24 `BONUS_COUNT_STEP`s would land on a machine that has just been talking for five seconds |
| **a hole-bonus window opening** at the 5th hit | [gameplay.md §6](../../../FlipperArchitecture/docs/gameplay.md#6-the-hole-bonuses-and-the-captive-balls) | the 5th hit raises `HOLEBONUS_*_NORMAL_HIT` like the four before it, and six lamps starting to blink is the machine saying so with light. A separate cue here is a design decision nobody has argued yet |
| **a hole-bonus window expiring** uncollected | same | **the honest gap.** Losing 55 000 to a timer is the harshest thing the rules do and the machine says nothing about it. It wants a cue and none was added, because inventing one costs four sets a file each and nobody has watched a window close |
| **the thunderstrike** — three bumpers inside a second, +500 | [gameplay.md §8](../../../FlipperArchitecture/docs/gameplay.md#8-the-side-lanes-the-sidebars-and-the-bumpers) | it is announced in light — four white flashes of the backlight — and it arrives on the back of three `BUMPER` raises, which is already the most-fired cue on the machine |
