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
- **A paragraph that continues the one above it belongs to it.** A block of prose or a numbered
  list that does not open with a claim is not a rule of its own — it is the rest of the rule above,
  and it is carried into the same file. `So a count of 25 shows five ladder lamps…` is the second
  half of the paragraph that says what the lamps stand for, and cutting it loose would leave a rule
  with its arithmetic missing.
- **A block that opens with an identifier rather than bold is still a rule**, when what follows is
  a claim: `` `BUNKER_LEFT` pays **100**, and starts multiball… `` is a rule about the left bunker.
- **A subsection that opens with a table, or with a paragraph that has no bold claim, is still a
  rule — and its title is the subsection's heading.** §13's *The displays* is a table and nothing
  else; *The indicator LEDs* is one unbolded paragraph. Both are rules, and reading the heading as
  the claim is the only thing that keeps them.
- **A fenced block that is not mermaid belongs to the rule above it.** §13 draws the four displays
  as a text block inside the rule that describes them. Mermaid is the exception, because a diagram
  of a whole section belongs to no single rule.
- **A fence with a blank line inside it is two blocks, and the second one closes it.** Track the
  fence across blocks rather than per block: a mermaid diagram with a gap in the middle otherwise
  leaves the cut inside the fence for the rest of the section, and every rule after it is dropped.
  This cost §11 a rule, and it was found by counting rather than by any check.
- **A heading, a mermaid or code fence, and a sentence that only points at another section are not
  rules, and they do not attach to anything.** Skip them and say so — a heading especially, because
  attaching one to the rule above it would put the next subsection's title inside it.

## Doing it

1. Read the section in the checkout beside this one, on whatever branch it is on, and note the
   commit: `git -C ../<checkout> rev-parse --short HEAD`. That is `as-of`.
2. Find the last rule number: `ls raw/rules/ | sort | tail -1`. Continue from it.
3. For each rule, in document order: the file `raw/rules/NNNN-<slug>.md`, the front matter, the
   source as a link on the first line — the section's anchor, as the root's `check_anchors.py`
   slugs it — then the paragraph **verbatim**. The slug is the bold sentence, lower-cased, at most
   eight words. `body:` is `game` for gameplay.md and the state documents, `1987` for machine.md,
   `vpx`, `simulator` or `cabinet` for a body's document.
   **The title is plain text**: the claim with its bold and italics dropped, a link reduced to its
   words, no trailing full stop, and cut at a clause if it runs past about 96 characters. A title
   carrying a link is a link the checks will follow out of the front matter and find nothing at.
   **Every relative link inside the paragraph is re-pointed across the seam**, and nothing else in
   it changes. A bare anchor `(#12-the-ball-…)` points at the document itself and becomes
   `(../../../FlipperArchitecture/docs/gameplay.md#12-…)`; a sibling document `(machine.md#14-…)`
   becomes `(../../../FlipperArchitecture/docs/machine.md#14-…)`. The link *text* is untouched, and
   the `diff` in step 4 allows exactly these substitutions and no others.
4. `diff` each file's body against the paragraph it came from. Empty, or the cut is wrong.
5. One commit for the cut: *cut gameplay.md §3 into rules 0003–0010* — and one line in
   `wiki/log.md`: `<when>  cut  §3 of gameplay.md  0003–0010`.

## What not to do

- Do not paraphrase, shorten, or fix a paragraph. A rule that seems wrong is cut as it is; the
  wrongness is a finding for the document, next door.
- Do not ingest. Do not touch `wiki/` beyond the log line.
- Do not renumber. A number, once given, is an identity.
