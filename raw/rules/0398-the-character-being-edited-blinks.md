---
rule: 0398
title: The character being edited blinks, and the machine blinks it itself
source: FlipperEngine/docs/states/highscore.md § HighscoreMachine — What is on the glass
as-of: 0e97ce3
body: game
supersedes:
---
[highscore.md § HighscoreMachine — What is on the glass](../../../FlipperEngine/docs/states/highscore.md#what-is-on-the-glass)

**The character being edited blinks, and the machine blinks it itself** — one `TimeTrigger`, a
boolean and an `ActionDisplayDigits` per phase. `ActionAlternate` in the `ActionProcessor` does not
work here: continuous actions are keyed by address and a second request for an address that already
has one is dropped, so every keypress would be a deactivate and an activate. Owning it also resets
the phase to lit on every keypress, so the character you stepped to is on the instant you step to it.
