---
rule: 0421
title: Nothing remembers which lamps are lit
source: FlipperEngine/docs/states/credits.md § CreditsMachine — The light show
as-of: 0e97ce3
body: game
supersedes:
---
[credits.md § CreditsMachine — The light show](../../../FlipperEngine/docs/states/credits.md#the-light-show)

**Nothing remembers which lamps are lit**, and that is the whole trick. Two draws out of the 48, one
written on and one written off; whether either lamp was already in that state does not matter to
anyone and would cost a byte of state per lamp to find out. One on and one off per cycle also holds
the playfield at roughly half lit on its own, with no counting — a balance a bookkeeping version
would have had to work for. The lamp block is addressed as the contiguous range 181–228 rather than
by name: `Intro` names each lamp because its sweep runs in playfield order, and this show has no
order at all.
