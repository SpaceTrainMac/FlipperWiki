---
name: wiki-query
description: Answer a question about the Space Train machine from FlipperWiki's pages first and its rule files second, with citations, and file the answer as a page when it needed more than one page to give. Use when someone asks what a lamp means, what just happened at the glass, what to do now, or any question about the game's rules, its ceremonies, its displays or how one body differs from another.
---

# Answering from the wiki

**Pages first, rules second, documents never.** The wiki exists so that an answer is not derived
from the raw layer every time; an answer built from the documents next door improves nothing and
bypasses every citation the pages carry.

## Doing it

1. `wiki/index.md` first — it is the catalogue, one line per page. Pick the pages whose title,
   summary or category match; open them; follow their links.
2. If the pages are silent, search `raw/rules/` for the names in the question. A rule with no page
   is a finding: say so, and offer to ingest it.
3. Answer in the voice of the page — bold claim, then the argument — and cite every sentence as
   the pages do, by rule number, as links. A `1987` rule is quoted with *1987* in the sentence; a
   body's rule with the body.
4. If the answer needed **more than one page**, file it: `wiki/questions/YYYYMMDD-<slug>.md`,
   `type: question`, citing the *pages* it joined — never rule files directly, so that it goes
   stale exactly when the pages do. Add its line to the index and one to the log:
   `<when>  query   filed questions/YYYYMMDD-<slug>`. Commit: *filed question: <slug>*.
   An answer one page gave is a link to that page and is not filed.

## What not to do

- Do not answer from gameplay.md, machine.md or any document beside this checkout. If the wiki
  cannot answer, the wiki lacks a rule, and that is the answer.
- Do not state anything a page or rule does not; say `TBC` and what would settle it.
- Do not edit a page while answering. A page that turns out wrong is a lint finding.
