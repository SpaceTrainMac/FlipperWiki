---
rule: 0241
title: A digit is seven segments
source: FlipperSimulator/docs/using-the-simulator.md § 2. The first five minutes - Reading the picture
as-of: 4644649
body: simulator
supersedes:
---
[using-the-simulator.md § 2. The first five minutes - Reading the picture](../../../FlipperSimulator/docs/using-the-simulator.md#reading-the-picture)

- **A digit is seven segments**, lit from the byte the engine sent rather than from a number the page
  was told. The text under the backglass runs those bytes back through an inverse map, so a glyph
  that is not a digit reads as whatever it most nearly is.
