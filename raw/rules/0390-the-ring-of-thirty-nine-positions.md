---
rule: 0390
title: Name entry
source: FlipperEngine/docs/states/highscore.md § HighscoreMachine — Name entry
as-of: 0e97ce3
body: game
supersedes:
---
[highscore.md § HighscoreMachine — Name entry](../../../FlipperEngine/docs/states/highscore.md#name-entry)

`NameEntry` (`src/machines/nameEntry.hpp`) is the whole interaction, with no hardware in it: a ring of
thirty-nine positions, walked in both directions and wrapping at both ends.

```text
   [rub out]  [space]  A B C … Z  0 1 2 … 9  -
```

| Button | Does |
|---|---|
| `BUTTON_LEFT` | the previous position in the ring |
| `BUTTON_RIGHT` | the next one |
| `BUTTON_START` | confirms the character and moves along one |
