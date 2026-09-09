---
rule: 0011
title: Ten quantities, and everything below is one of them changing.
source: FlipperArchitecture/docs/gameplay.md § 1. What the machine keeps track of
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 1. What the machine keeps track of](../../../FlipperArchitecture/docs/gameplay.md#1-what-the-machine-keeps-track-of)

**Ten quantities, and everything below is one of them changing.** Each is per player — four players
are four independent games sharing one playfield, and nothing one player lights ever pays for
another.

| Quantity | Range | Lives for | Shown on |
|---|---|---|---|
| **The score** | 0 – 9 999 999 | the game | that player's 6-digit display |
| **The turn score** | 0 upward — six digits is the *display*, not the range ([§13](../../../FlipperArchitecture/docs/gameplay.md#13-what-the-machine-shows)) | one turn | the `MATCH` display, the fifth 6-digit one |
| **The bonus count** | 0 – 39 | one ball | the bottom ladder and Super Bonus — **lamps only** |
| **Total bank completions** | 0 – 50, no further effect past 50 | the game | nothing directly — `X_BON` flags the 20 s window it opens at the 40th and 50th |
| **Three multipliers** | ×1 – ×3 each | the game | `X2_BOT` / `X3_BOT`, and one pair beside each hole ladder |
| **Two hole-bonus ladders** | 0 – 5 rungs, plus an armed marker | one ball, but a redemption window can outlive a hit | five lamps and a `HOLE BONUS 30000` lamp a side |
| **Two hole-redemption counts** | 0 – 3, no further effect past 3, one a side | the game | nothing directly — that side's six lamps blinking mark an open window |
| **Four lit awards** | lit or not | one ball | `SPECIAL` ×2, `EXTRA BALL` top, `EXTRA BALL` right |
| **Extra balls in hand** | 0 upward | the turn | the two-digit field, printed `CREDITS` |
| **Extra balls won** | 0 upward, never decreasing | the game | nothing during a game — the `MATCH` display shows it afterwards, with `EXTRA BALL` right lit |
