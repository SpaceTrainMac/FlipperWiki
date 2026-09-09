---
rule: 0379
title: The same scene attract mode runs, in a second place
source: FlipperEngine/docs/states/show-highscore.md § ShowHighscore — the table after the game
as-of: 0e97ce3
body: game
supersedes:
---
[show-highscore.md § ShowHighscore — the table after the game](../../../FlipperEngine/docs/states/show-highscore.md#showhighscore--the-table-after-the-game)


**Every way out is `Credits`, whatever the scene reports.** It can end three ways — the second pass
finishing, `BUTTON_START`, the setup gesture — and in attract mode two of those are exits. Here they
are not, and that is `MasterControlProcess`'s doing rather than the machine's: the game is over and
