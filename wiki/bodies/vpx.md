---
title: The Visual Pinball table
type: body
aliases: [vpx, VPX, the table, the Visual Pinball table, the simulated table, VPinball]
body: vpx
---
# The Visual Pinball table

**One of the three machines anybody can actually play, and the only one where the cabinet is a
keyboard** ([0214](../../raw/rules/0214-the-keys-are-vpxs-own-defaults.md)). Everything the wiki says about the game is true here; what is different is how
you reach it.

## What each key is

| Key | |
|---|---|
| **Left Shift** / **Right Shift** | [the flippers](../things/flipper-buttons.md) |
| **Enter** | [the plunger](../things/plunger.md) — hold to pull back, release to fire |
| **1** or **S** | [start](../things/start-button.md) — the machine's own button, and **once a game is running it does nothing** |
| **Z** / **`/`** / **Space** | nudge left, right, forward |
| **Esc** | leave — use it rather than killing the player |

*(the table is using-the-table.md §4's, rendered for a player ([0214](../../raw/rules/0214-the-keys-are-vpxs-own-defaults.md)))*

**They are VPX's own defaults and this table changes none of them** ([0214](../../raw/rules/0214-the-keys-are-vpxs-own-defaults.md)). `1` is VPX's Start
key and follows anything you rebind it to; `S` is the letter itself, and that one is this table's
([0214](../../raw/rules/0214-the-keys-are-vpxs-own-defaults.md)).

**The start key is player select's, and a game in progress does not read it** ([0215](../../raw/rules/0215-the-start-button-belongs-to-player-select.md)). The press
that ends player select is what serves the first ball; after that the machine serves every ball
itself. **This is worth saying twice because the table's own manual said the opposite until
2026-09-05**, describing a saved ball that waited for a press — behaviour the engine had until that
afternoon and does not have now ([0215](../../raw/rules/0215-the-start-button-belongs-to-player-select.md)).

**[Drain protection](../concepts/drain-protection.md) is the same 15 seconds here, and the ball is
back in about 400 ms** ([0216](../../raw/rules/0216-a-ball-that-drains-in-the-first-fifteen-seconds-is-given-back.md)). The window opens as the ball passes out-fire and lasts once a
turn; a drain inside it does not end the turn, and the ejector fires again as soon as the trough
has a ball under it ([0216](../../raw/rules/0216-a-ball-that-drains-in-the-first-fifteen-seconds-is-given-back.md)).

**A ball that sits in the trough and stays there is a fault, not a rule** ([0217](../../raw/rules/0217-a-ball-sitting-in-the-trough-is-a-fault-not-a-rule.md)). It is what this
table did until 2026-09-05: the engine waited thirty seconds for a press nobody knew to make, and
the only thing anywhere that said so was one lamp among forty-eight ([0217](../../raw/rules/0217-a-ball-sitting-in-the-trough-is-a-fault-not-a-rule.md)). It was fixed in the
engine and pinned by a test, so if you ever see it again it is a defect worth reporting ([0217](../../raw/rules/0217-a-ball-sitting-in-the-trough-is-a-fault-not-a-rule.md)).

**The flipper keys are VPX's own, and nothing about the bridge to the engine can make them feel
bad** ([0218](../../raw/rules/0218-your-flipper-keys-are-vpxs-own.md)). The ball, the flipper and the key are all inside VPX's own loop, exactly as the
cabinet's buttons and coils are wired to each other rather than through the game — the engine's
only say is the same relay ([0218](../../raw/rules/0218-your-flipper-keys-are-vpxs-own.md)).

**Every other key VPX offers reaches nothing** ([0219](../../raw/rules/0219-the-other-keys-vpx-offers-reach-nothing.md)). There is no coin switch anywhere in this
machine's matrix, so the credit keys close nothing at all; and the tilt key is VPX's own, which is
[not the same thing as a tilt on the cabinet](../concepts/tilt.md) ([0219](../../raw/rules/0219-the-other-keys-vpx-offers-reach-nothing.md)).
