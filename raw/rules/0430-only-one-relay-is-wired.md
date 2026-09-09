---
rule: 0430
title: Addresses 241 to 245, and only one relay is wired
source: FlipperArchitecture/docs/hardware.md § 7. Relays
as-of: 0804fe1
body: game
supersedes:
---
[hardware.md § 7. Relays](../../../FlipperArchitecture/docs/hardware.md#7-relays)

Addresses **241 – 245**. Data: `0` = off, anything else = on.

| Addr | Schematic | Code identifier | Purpose |
|---|---|---|---|
| 241 | Relais 1 | `FRA_NO_PADDLE_MODE` | No-Paddle mode — disables the flippers |
| 242 – 245 | Relais 2 – 5 | *(commented out)* | *n.v.* — not wired |
