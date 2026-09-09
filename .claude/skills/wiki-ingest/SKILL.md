---
name: wiki-ingest
description: Process one rule from FlipperWiki/raw/rules/ into the wiki - read it, say the takeaways, write its summary page, update every page it touches, the index and the log, and commit - the way Karpathy's LLM Wiki ingests one source. Use when the user says "ingest rule NNNN", "ingest the next rule", "process the rules of §N", or an observation has been added under raw/observations/.
---

# Ingesting one rule

**One rule, five outputs, one commit.** This is the gist's ingest applied to one raw file, and the
shape of every file it writes is [CLAUDE.md](../../../CLAUDE.md#a-page). Read that first.

## The five outputs, in order

1. **Read.** The rule file, `wiki/index.md`, and every existing page whose `aliases` or title
   name something the rule names — a lamp, a switch, a lane, a ceremony, a concept. Read the
   pages you will touch *before* writing, so you compound rather than staple.
2. **Takeaways.** Say, in the reply, three to eight lines: what the rule means at the glass, which
   names it touches, which pages that is, and whether it contradicts any page. **This is the
   review.** If a person says *no* to a line, the pages change before the commit.
3. **The summary page.** `wiki/rules/NNNN-<slug>.md`, `type: rule`: the rule at the glass, one or
   two paragraphs a player would want, citing the rule by number. Not a copy of the rule — the
   raw file is the copy.
4. **The pages it touches.** For every name the rule mentions:
   - a **thing** (`wiki/things/`) — a lamp, a switch, a coil, a display, an LED, the backlight,
     a captive ball, a bank. One page per thing a player sees as one thing; a group that reads as
     one is one page with every member in `aliases`.
   - a **concept** (`wiki/concepts/`) — M-A-C, the advance-bonus bank, the bonus count, a hole
     bonus, a multiplier, multiball, drain protection, the extra ball, the special.
   - a **moment** (`wiki/moments/`) — attract, player select, the serve, the end of a ball, the
     count, the transfer, the draw, name entry, the high score table, the credits.
   - a **body** (`wiki/bodies/`) — when the rule's `body` is not `game`, the paragraph goes on
     the body page and the thing pages get one sentence pointing there.

   Create a page that does not exist; **rewrite the paragraph** of one that does so it holds the
   old claim and the new one. Every sentence cites its rule as a link by number. A claim that is
   the sum of two rules cites both. A claim that no rule makes is not written.
5. **The index and the log.** Every new page gets its line in `wiki/index.md` under its category;
   a page whose summary changed gets its line rewritten. One line appended to `wiki/log.md`:
   `<YYYY-MM-DDTHH:MM>  ingest  NNNN  <the pages touched, comma-separated>`.

## The commit

One commit, the rule's pages and nothing else. Subject: *ingested rule NNNN, <title>: N pages*.
Body: the takeaways as spoken, then the pages by path. Check before committing that every link in
the pages you wrote resolves — a rule citation from `wiki/<dir>/` is two directories up, in
`../../raw/rules/`.

## An observation

An observation under `raw/observations/` is ingested the same way, with one difference: where it
disagrees with a rule, the rule's pages gain a paragraph opening **Watched.** that cites the
observation and the rule and decides nothing. A discrepancy is a finding for the document next
door; the takeaways say so.

## What not to do

- Do not edit a rule file. Ever. A wrong rule is a new rule with `supersedes:`.
- Do not write a sentence no rule supports, however obvious. Write `TBC` and what is missing.
- Do not append a second paragraph about a thing a page already has a paragraph about.
- Do not add front-matter fields. Four, and `aliases` is the only list.
- Do not ingest two rules in one commit.
- **Do not link to a page a later rule will create.** The link check refuses it, and rightly: a
  wiki that points forward is a wiki with dead links in it between two commits. Name the thing in
  words and let the rule that creates the page come back and point at it — and say so in both
  commits, so the second one knows what it owes the first.
- **Never re-run an ingest script from the top after a failure.** Reset the tree, then run *only*
  the rules that did not commit. A script that opens by creating a page will silently overwrite the
  paragraphs the rules after it added — which cost rule 0380 its paragraph on 2026-09-10, in a
  commit that looked clean.
