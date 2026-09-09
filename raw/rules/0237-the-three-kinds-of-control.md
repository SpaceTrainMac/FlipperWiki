---
rule: 0237
title: The three kinds of control, and why they look different
source: FlipperSimulator/docs/using-the-simulator.md § 2. The first five minutes - The three kinds of control, and why they look different
as-of: 4644649
body: simulator
supersedes:
---
[using-the-simulator.md § 2. The first five minutes - The three kinds of control, and why they look different](../../../FlipperSimulator/docs/using-the-simulator.md#the-three-kinds-of-control-and-why-they-look-different)

| Kind | How many | Behaves like |
|---|---|---|
| **Momentary** | most of them | One click closes and reopens — a target, a rollover, a slingshot. The release is held back to a later read so the closure gets a machine cycle to itself |
| **Toggle**, drawn with a blue ring | five | Both bunkers and the three ball-rest sensors. Click to close, click again to open, because a ball can hold them closed indefinitely |
| **Cabinet button**, drawn apart | three | Start and the two flipper buttons. **Held, not tapped** — they close on the way down and open on the way up |
