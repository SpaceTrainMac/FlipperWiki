---
rule: 0091
title: When every player is out of balls, the draw runs
source: FlipperArchitecture/docs/gameplay.md § 12. The ball, the turn and the game
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 12. The ball, the turn and the game](../../../FlipperArchitecture/docs/gameplay.md#12-the-ball-the-turn-and-the-game)

**When every player is out of balls, the draw runs.** A random two-digit number appears on the
`MATCH` display, and every player whose score ends in those two digits is given one more ball,
played in player order like any other turn. A score of nothing never wins. The width is the
operator's — one digit is a draw in ten, two is the classic draw in a hundred.
