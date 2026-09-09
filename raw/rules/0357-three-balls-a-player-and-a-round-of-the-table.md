---
rule: 0357
title: Three balls a player, and the rotation is a round of the table
source: FlipperEngine/docs/states/play.md § PlayMachine — inside the Play state
as-of: 0e97ce3
body: game
supersedes:
---
[play.md § PlayMachine — inside the Play state](../../../FlipperEngine/docs/states/play.md#playmachine--inside-the-play-state)

**Three balls a player**, a constant rather than a setting
([`Setup`](../../../FlipperEngine/docs/states/setup.md#what-is-still-not-in-it)) — and it is `GameMachine`'s constant, because balls owed is a fact
about the player. Ball 1 for everybody, then ball 2: the rotation is a round of the table rather than
one player playing out, which is what the four score displays side by side are for.
