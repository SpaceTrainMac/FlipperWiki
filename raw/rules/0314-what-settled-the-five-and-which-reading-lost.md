---
rule: 0314
title: What settled the five, and which reading lost
source: FlipperEngine/docs/sound.md § 4. The catalogue - What settled the five
as-of: 0e97ce3
body: game
supersedes:
---
[sound.md § 4. The catalogue - What settled the five](../../../FlipperEngine/docs/sound.md#what-settled-the-five)

**Five cues stood in this section as TBC**, each with two readings the name allowed and no rule to
choose between them. [gameplay.md](../../../FlipperArchitecture/docs/gameplay.md) is that rule set, and
the record that read it against this catalogue is
[FlipperSounds §3](../../../FlipperSounds/docs/concepts/done/20260904-the-cues-the-rules-ask-for.md).
**What is kept here is which reading lost**, because a cue that is settled twice is a cue somebody
will settle a third way.

| Cue | Was | Settled as | What decided it |
|---|---|---|---|
| `NO_MORE_EXTRABALL` | *earned and refused*, or *the last one has been played off* | **the second** — the turn ending on a drain with the field at zero | D35 made the two-digit field *extra balls in hand*. Nothing refuses an extra ball on this machine, so the first reading has no event behind it |
| `MAIN_BONUS_ONE_LIGHT` | *the ladder is complete*, or *one lamp still unlit* | **the first** — the count reaching 39 | The name reads more naturally as the second and the vocabulary needed the first. A ladder has exactly one terminal state; *one short of the end* is not a state the rules mark, light or pay for |
| `TOPLANES_SELECT_BONUS` | the lane change, *or no sound at all* | **the lane change, rate-limited** | The objection was never the mapping, it was the rate. A minimum interval answers it and losing the only cue the top lanes have for a decision a player makes does not. **The interval was never built**: when the cue was raised on 2026-09-08 the buttons turned out to be flanks, so the rate the objection feared does not exist (the row above) |
| `TOPLANES_SUPERBONUS` | an unbuilt *combination* chain, or *M-A-C completed* | **M-A-C completing, and `M`/`C` paying** | D43 gave the upper bank no targets of its own. Nothing is left up there for the cue to mean, and the completion is the only Super-Bonus-shaped event that happens there |
| `HOLEBONUS_*_BONUS30K_A` … `_F` | a six-step escalation, or six alternates in rotation | **six items counted out** — five rungs and the marker | The escalation was the reading available before D30, when a redemption paid one item. Alternates already have a mechanism — a list value — and six *named* cues is not it. The original player had five labelled `bonus30k` triggers and one unlabelled, which is where six lettered cues came from |
