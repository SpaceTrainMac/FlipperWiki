---
rule: 0146
title: BUTTON_START — what closing it does
source: FlipperArchitecture/docs/gameplay.md § 2. Every switch, and what closing it does
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 2. Every switch, and what closing it does](../../../FlipperArchitecture/docs/gameplay.md#2-every-switch-and-what-closing-it-does)

| Switch | Pays | Advances | Collects |
|---|---|---|---|
| `BUTTON_START` | — | starts a game and adds players, **at player select and nowhere else**. A game in progress does not read it ([§12](../../../FlipperArchitecture/docs/gameplay.md#12-the-ball-the-turn-and-the-game)) | — |
