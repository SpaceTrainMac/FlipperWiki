---
rule: 0317
title: These name when they play, which is the role rather than the content
source: FlipperEngine/docs/sound.md § 4. The catalogue - Music, 3 cues
as-of: 0e97ce3
body: game
supersedes:
---
[sound.md § 4. The catalogue - Music, 3 cues](../../../FlipperEngine/docs/sound.md#music--music-3-cues)

**These name *when* they play**, which is the role rather than the content
([§5](../../../FlipperEngine/docs/sound.md#5-naming-what-a-cue-is-for-versus-what-it-is)) — and only `GAME_OVER_THEME` is raised, by
`GameOverMachine` beside the `GAME_OVER` effect; for the other two *when* is still an intention.
Whoever raises one should know what it does to the jukebox: it cuts the current
song off, and when it ends the jukebox starts **the next entry in the playlist**, not the song that
was interrupted ([the two users](../../../FlipperEngine/docs/concepts/done/20260812-jukebox.md#the-music-channel-has-two-users)).
