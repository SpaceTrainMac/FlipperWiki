---
rule: 0438
title: Adding one later is cheap and adding one now is not free
source: FlipperEngine/docs/sound.md § 4. The catalogue - Four events with no cue
as-of: be47236
body: game
supersedes: 0316
---
[sound.md § 4. The catalogue - Four events with no cue](../../../FlipperEngine/docs/sound.md#four-events-with-no-cue-and-why-that-is-not-eleven-more)

**Adding one later is cheap and adding one now is not free**, which is the whole argument: a cue is
an enum here, a key in five manifests, a score in four generators and a hand-found file in the
fifth. **A cue with no entry in a `sounds.json` is silent rather than fatal**, so the enum can grow
whenever a rule earns it.
