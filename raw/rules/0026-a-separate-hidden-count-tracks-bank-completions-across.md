---
rule: 0026
title: A separate, hidden count tracks bank completions across the whole game, not this ball's ladder
source: FlipperArchitecture/docs/gameplay.md § 5. The bonus count
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 5. The bonus count](../../../FlipperArchitecture/docs/gameplay.md#5-the-bonus-count)

**A separate, hidden count tracks bank completions across the whole game, not this ball's ladder.**
Every completion advances both at once, but only the ladder above resets each ball and caps at 39;
the hidden one never resets, so a player's 40th completion can land on any ball of the game and
still be the same event — the one `X_BON`'s 20 s window in [§7](../../../FlipperArchitecture/docs/gameplay.md#7-the-three-multipliers) is
watching for.
