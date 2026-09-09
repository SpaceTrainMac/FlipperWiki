---
rule: 0300
title: Each side is a five-hit build and then a timed all-or-nothing redemption
source: FlipperEngine/docs/sound.md § 4. The catalogue - Effects, The captive balls, hole bonus
as-of: 0e97ce3
body: game
supersedes:
---
[sound.md § 4. The catalogue - Effects, The captive balls, hole bonus](../../../FlipperEngine/docs/sound.md#the-captive-balls--hole-bonus)

**Each side is a five-hit build and then a timed all-or-nothing redemption**
([gameplay.md §6](../../../FlipperArchitecture/docs/gameplay.md#6-the-hole-bonuses-and-the-captive-balls)):
rungs 1–4 light their lamps, the 5th lights the fifth rung *and* that side's `HOLE BONUS 30000` and
starts a 30-second window, and redeeming inside it — at that side's own bunker or at the twin again
— **pays the five rungs and the marker together** and resets the ladder. **The two sides are
symmetric**, which is why the left has six lettered `BONUS30K` cues since 2026-09-04 and had one
before: a redemption is six things to count out on either side.
