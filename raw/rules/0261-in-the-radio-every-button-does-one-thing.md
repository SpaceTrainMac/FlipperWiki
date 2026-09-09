---
rule: 0261
title: Every button does one thing
source: FlipperEngine/docs/cabinet.md § 2. The service menu - The radio, and the three buttons in it
as-of: 0e97ce3
body: cabinet
supersedes:
---
[cabinet.md § 2. The service menu - The radio, and the three buttons in it](../../../FlipperEngine/docs/cabinet.md#the-radio-and-the-three-buttons-in-it)

You get there three ways: wait, hold the right flipper alone for nine seconds in attract mode, or use
`RADIO TEST` in the menu. Once there, **every button does one thing**:

| Button | Does |
|---|---|
| start | starts a game, exactly as it would from attract mode |
| right flipper | **the next station** in `radioStations`, wrapping. It starts playing at once, its name goes on the glass, and `settings.json` is rewritten on the press |
| left flipper, **tapped** | back to attract mode |
| left flipper, **held** | **the volume.** Hold it and the number climbs; let go and that is the volume |
| both flippers, nine seconds | the service menu, the same gesture as everywhere else |
