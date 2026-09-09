---
rule: 0333
title: Two entries are on the glass at once, and the window slides from the worst place towards the best
source: FlipperEngine/docs/states/intro.md § IntroMachine — The high score scene
as-of: 0e97ce3
body: game
supersedes:
---
[intro.md § IntroMachine — The high score scene](../../../FlipperEngine/docs/states/intro.md#the-high-score-scene)

Two entries are on the glass at once, and the window slides **from the worst place towards the
best** — 9th over 10th, then 8th over 9th, ending on 1st over 2nd. Nine pages for a full table of
ten, `PAGE_MS` each. Every page but the ends shows a name twice, once arriving at the bottom and
once moving up, which is what makes it read as one list travelling rather than as nine unrelated
screens; ending on first place leaves the score to beat as the last thing on the glass. Each entry
sits across one row of two displays — the name on the left, the score on the right — and `MATCH`
carries `SCORES` throughout so a glance says what the numbers are.
