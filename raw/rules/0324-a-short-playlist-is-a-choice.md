---
rule: 0324
title: A short playlist is a choice and an empty one is legitimate
source: FlipperEngine/docs/sound.md § 4. The catalogue - Songs, a playlist
as-of: 0e97ce3
body: game
supersedes:
---
[sound.md § 4. The catalogue - Songs, a playlist](../../../FlipperEngine/docs/sound.md#songs--songs-a-playlist)

**A short playlist is a choice and an empty one is legitimate** — a sound set with no songs is a
sound set. So `songs` has no unmapped half to report: only a path naming a file that is not on disk
counts against it, and that stays fatal like any other missing file.
