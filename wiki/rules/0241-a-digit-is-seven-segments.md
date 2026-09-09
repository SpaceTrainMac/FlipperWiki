---
title: The page lights segments from the engine's own bytes, not from numbers
type: rule
aliases: []
body: simulator
---
# Rule 0241 — A digit is seven segments

**At the glass: what you see is what went on the wire.** Each digit is lit from the byte the engine
sent rather than from a number the page was given, and the text under the backglass reads those
bytes back through an inverse map — so a glyph that is not a digit shows as whatever it most
nearly is ([0241](../../raw/rules/0241-a-digit-is-seven-segments.md)). Pages: [the browser simulator](../bodies/simulator.md),
[what the glass shows](../concepts/what-the-glass-shows.md).
