# CLAUDE.md — the schema

**This file is the schema of the wiki: how it is laid out, what a file in it looks like, and what
the four operations do.** It is the document an LLM reads first, and it is a rulebook rather than a
map, which is the opposite of the engine's `CLAUDE.md` next door — because here the LLM is the
writer. The reasoning is
[docs/concepts/open/20260909-a-wiki-for-whoever-is-at-the-glass.md](docs/concepts/open/20260909-a-wiki-for-whoever-is-at-the-glass.md);
[README.md](README.md) is the same rules for a person.

## What this is

A wiki for whoever is at the glass of the Space Train (MAC, 1987) — the cabinet, the Visual
Pinball table, or the browser simulator — answering *what does that lamp mean*, *what just
happened*, *what do I do now*. Karpathy's LLM Wiki pattern: raw sources the LLM never edits, a
wiki the LLM owns entirely, this schema. **The raw sources are the rules of the game, one file
each, added one at a time.** A person adds the next rule, asks questions and reads; the LLM does
everything else.

## Layout

```
raw/rules/NNNN-<slug>.md        one rule each, verbatim with provenance above it - never edited
raw/observations/YYYYMMDD-<body>.md   what a person saw at which glass - never edited
wiki/index.md                   every page, one line each, by category - updated on every ingest
wiki/log.md                     append-only: what happened and when
wiki/rules/NNNN-<slug>.md       one summary page per rule: the rule at the glass
wiki/things/<slug>.md           a lamp, a switch, a coil, a display, an LED, the backlight
wiki/moments/<slug>.md          attract, player select, the serve, the count, the draw, name entry, ...
wiki/concepts/<slug>.md         M-A-C, the bank, the count, the hole bonuses, the multipliers, ...
wiki/bodies/<slug>.md           cabinet, vpx, simulator, 1987
wiki/questions/YYYYMMDD-<slug>.md   an answer that was filed
```

A directory that does not exist yet is created by the first ingest that needs it.

## A rule file

```markdown
---
rule: 0031
title: M and C pay for as long as the player leaves A alone
source: FlipperArchitecture/docs/gameplay.md § 3. M-A-C
as-of: cb52384                # the commit of that checkout the text was copied from
body: game                    # game | cabinet | vpx | simulator | 1987
supersedes:                   # a rule number, when this one replaces an earlier one
---
[gameplay.md § 3. M-A-C](../../../FlipperArchitecture/docs/gameplay.md#3-m-a-c)

**The paragraph, exactly as the document has it.** Verbatim, links and all.
```

- **Verbatim.** A paraphrase in the raw layer is the LLM's first opinion disguised as a source.
- **Never edited.** When the machine changes, a new rule is appended with `supersedes:` naming the
  old one. Lint keys on that field.
- **Numbered in the order added**, four digits. The number is an identity, not a ranking.
- **The first line is the source as a link**, so that the root's `check_anchors.py` verifies the
  section exists. `source:` is the same fact for the LLM.
- A person may write a rule: `source: RooL, at the cabinet, 2026-09-14` is legal provenance.

## A page

```markdown
---
title: M-A-C
type: concept                 # rule | thing | moment | concept | body | question
aliases: [MAC, M · A · C, the top lanes]
body: game                    # game | cabinet | vpx | simulator | 1987
---
# M-A-C

**Every paragraph opens with a bold sentence that is the claim.** The rest is the argument, and
every sentence cites the rule it rests on by number, as a link:
([0031](../../raw/rules/0031-m-and-c-pay-for-as-long-as-a-is-left-alone.md)).
```

- **Four front-matter fields and no more.** `sources:` would be a second copy of the citations.
- **`aliases` is where a page claims names.** Every switch, lamp, LED, display, coil, backlight
  channel, award, cue and state of the machine must be claimed by exactly one page; lint counts.
  A group that a player sees as one thing is one page — the six hole-bonus lamps, the four
  `ADVANCE BONUS` targets.
- **A page says what its rules say and nothing more.** A sentence with no rule behind it is a
  lint finding. Where a player's question has no rule: `TODO` (input no source can recover),
  `TBD` (a decision not taken), `TBC` (only the machine can confirm it) — in the text, with what is
  missing.
- **A `1987` rule is quoted with *1987* in the sentence**; a body's rule with the body. A page
  whose `body` is `game` carries a body's difference as one sentence pointing at the body page.
- **Links are markdown paths, never `[[wikilinks]]`**, into this tree or into the checkouts
  beside it — never a URL to this project.
- **Compound, do not staple.** A later rule that touches a paragraph rewrites that paragraph to
  hold both claims; it does not append a second paragraph about the same thing.

## `wiki/index.md`

By category, one line per page — the title as a link, a dash, a one-line summary. Every page is
in it; every line in it is a page. Updated on every ingest, by the LLM.

## `wiki/log.md`

Append-only. One line per operation:

```
2026-09-09T22:14  ingest  0031  concepts/m-a-c, things/30k-top-lamps, rules/0031
2026-09-10T09:02  query   filed questions/20260910-why-did-the-backbox-go-dark
2026-09-10T18:40  lint    3 findings, 1 page written
```

## The four operations

Each is a skill in `.claude/skills/`, and the skill is the workflow; this file is the shape.

| Operation | Skill | In one line |
|---|---|---|
| cut | `wiki-cut` | one section of a document into rule files, verbatim, **nothing processed** |
| ingest | `wiki-ingest` | one rule: read, takeaways, the summary page, every page it touches, the index, the log — one commit |
| query | `wiki-query` | answer from pages first, rule files second, with citations; file the answer if it needed more than one page |
| lint | `wiki-lint` | contradictions, superseded claims, orphans, unclaimed names, uncited sentences, index integrity — findings into the log |

**One commit per ingest, and its subject is the log line in words**: *ingested rule 0031, M and C
pay for as long as A is left alone: four pages*. The body carries the takeaways.

## What is never here

- A copy of a document that is not a rule. The documents live in the checkouts beside this one.
- The machine's own files — `settings.json`, the high score file, the odometer, the state log. What
  they mean is a rule; their contents are not.
- An edit to any source. The arrow points one way. A rule that is wrong because its document is
  wrong is a finding next door and a new rule here.
