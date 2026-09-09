---
rule: 0246
title: Seven of the eighteen are editable at the machine
source: FlipperEngine/docs/cabinet.md § 1. The settings file
as-of: 0e97ce3
body: cabinet
supersedes:
---
[cabinet.md § 1. The settings file](../../../FlipperEngine/docs/cabinet.md#1-the-settings-file)

**Seven of the eighteen are editable at the machine**, without a keyboard or an SSH session: `volume`,
`soundSet`, `sfxMode`, `jukeboxMode`, `radio`, `radioIdleSeconds` and `creditsSeconds` are what the
service menu offers, and it writes them back to this file. See [§2](../../../FlipperEngine/docs/cabinet.md#2-the-service-menu). `radio` has a second
way in: **the right flipper steps stations while the radio is playing**, and each press is written
straight back to this file ([§2](../../../FlipperEngine/docs/cabinet.md#the-radio-and-the-three-buttons-in-it)).
