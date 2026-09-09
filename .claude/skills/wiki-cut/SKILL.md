---
name: wiki-cut
description: Cut one section of a document into rule files under FlipperWiki/raw/rules/ - one bold-led paragraph or one table row per file, verbatim, with its provenance above it - and process nothing. Use when the user says "cut §N", "make rules out of", "add the rules of <section>", or names a section of gameplay.md, machine.md, using-the-table.md or a state document to bring into the wiki.
---

# Cutting a section into rules

**A cut is a person's act with an LLM's hands, and it is not an ingest.** It turns one section of
a document into rule files and stops; each rule's ingest is a separate, later step with its own
takeaways, so that a person can look at the cut before the wiki is built from it. The shape of a
rule file is [CLAUDE.md](../../../CLAUDE.md#a-rule-file) and is not restated here.

## The grain

- **One bold-led paragraph is one rule.** Every paragraph in the project's documents opens with a
  bold sentence that is the claim; that is the unit. A paragraph that carries a table carries it
  whole.
- **One table row is one rule** where a section is a table — gameplay.md §2 (every switch) and
  §14 (every award). The row goes in with its header row above it, so it reads.
- **A mermaid block, a lead sentence with no claim, and a sentence that only points at another
  section are not rules.** Skip them and say so.

## Doing it

1. Read the section in the checkout beside this one, on whatever branch it is on, and note the
   commit: `git -C ../<checkout> rev-parse --short HEAD`. That is `as-of`.
2. Find the last rule number: `ls raw/rules/ | sort | tail -1`. Continue from it.
3. For each rule, in document order: the file `raw/rules/NNNN-<slug>.md`, the front matter, the
   source as a link on the first line — the section's anchor, as the root's `check_anchors.py`
   slugs it — then the paragraph **verbatim**. The slug is the bold sentence, lower-cased, at most
   eight words. `body:` is `game` for gameplay.md and the state documents, `1987` for machine.md,
   `vpx`, `simulator` or `cabinet` for a body's document.
   **A link inside the paragraph that points at the document itself** — `(#12-the-ball-…)` — is
   re-pointed at the document across the seam, `(../../../FlipperArchitecture/docs/gameplay.md#12-…)`;
   the words do not change, and the `diff` in step 4 allows exactly that.
4. `diff` each file's body against the paragraph it came from. Empty, or the cut is wrong.
5. One commit for the cut: *cut gameplay.md §3 into rules 0003–0010* — and one line in
   `wiki/log.md`: `<when>  cut  §3 of gameplay.md  0003–0010`.

## What not to do

- Do not paraphrase, shorten, or fix a paragraph. A rule that seems wrong is cut as it is; the
  wrongness is a finding for the document, next door.
- Do not ingest. Do not touch `wiki/` beyond the log line.
- Do not renumber. A number, once given, is an identity.
