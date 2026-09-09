---
rule: 0403
title: No special music
source: FlipperEngine/docs/states/highscore.md § HighscoreMachine — The table is written after every name
as-of: 0e97ce3
body: game
supersedes:
---
[highscore.md § HighscoreMachine — The table is written after every name](../../../FlipperEngine/docs/states/highscore.md#the-table-is-written-after-every-name)

**No special music.** `startOrContinue()` on the way in like every other state;
`SOUND_MUSIC_HIGHSCORE_THEME` belongs to the credits roll, which is long enough to carry a theme.
One `SOUND_SFX_BUMPER` per *confirmed* character, and silence while stepping.
