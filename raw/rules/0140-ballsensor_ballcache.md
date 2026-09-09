---
rule: 0140
title: BALLSENSOR_BALLCACHE — what closing it does
source: FlipperArchitecture/docs/gameplay.md § 2. Every switch, and what closing it does
as-of: 0804fe1
body: game
supersedes:
---
[gameplay.md § 2. Every switch, and what closing it does](../../../FlipperArchitecture/docs/gameplay.md#2-every-switch-and-what-closing-it-does)

| Switch | Pays | Advances | Collects |
|---|---|---|---|
| `BALLSENSOR_BALLCACHE` | — | **the drain** — a returning ball reaches the two-ball store here; a pulse is one ball home, a held contact is every ball home and the turn over ([§12](../../../FlipperArchitecture/docs/gameplay.md#12-the-ball-the-turn-and-the-game)) | — |
