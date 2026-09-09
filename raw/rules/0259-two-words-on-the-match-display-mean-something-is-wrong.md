---
rule: 0259
title: Two words on the MATCH display mean something is wrong
source: FlipperEngine/docs/cabinet.md § 2. The service menu
as-of: 0e97ce3
body: cabinet
supersedes:
---
[cabinet.md § 2. The service menu](../../../FlipperEngine/docs/cabinet.md#2-the-service-menu)

**Two words on the `MATCH` display mean something is wrong:**

| Shows | Means |
|---|---|
| `REBOOT` | the sound set you chose is not the one this process started with. Restart `mcp` for it to take effect |
| `NOSAVE` | `settings.json` **or** `highscores.csv` could not be written — a read-only card, a full disk, or a file owned by another user. The values are live for this run and will be gone after a power cycle. The reason is on stderr |
