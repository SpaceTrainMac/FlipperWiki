---
rule: 0322
title: Not cues: songs is an array of paths, addressed by index
source: FlipperEngine/docs/sound.md § 4. The catalogue - Songs, a playlist
as-of: 0e97ce3
body: game
supersedes:
---
[sound.md § 4. The catalogue - Songs, a playlist](../../../FlipperEngine/docs/sound.md#songs--songs-a-playlist)

**Not cues.** `songs` is a JSON **array of paths**, and a song is addressed by its position in it —
`ActionSong(3)` plays the fourth entry. There are no names, so there is no table here to keep in step
with an enum; there is no enum. Order is meaningful, because it is what the jukebox's `order` mode
plays.

```json
"songs": [
  "bttf/bttf_theme.mp3",
  "star-wars/star-wars-theme-song.mp3",
  "macgyver/MacGyver.mp3"
]
```
