---
name: wiki-lint
description: Health-check FlipperWiki - contradictions between pages, claims a superseded rule made, orphan pages, names of the machine with no page, sentences with no rule behind them, and index integrity - and write the findings into wiki/log.md. Use when the user says "lint the wiki", "is the wiki consistent", "what is the wiki missing", or after a batch of ingests.
---

# Linting the wiki

**A lint pass is a question put to an LLM, and nothing here gates.** The root's `check_links.py`
and `check_anchors.py` gate links once the wiki has its row in `repositories.json`; everything
below is a finding written down and, where a finding is a page to write, the page.

## The questions, in order

| Question | How |
|---|---|
| **Do two pages contradict each other?** | Read every page that names the same thing — the index groups them. A value, a lamp, a timing stated differently on two pages is a finding naming both and the rules each cites |
| **Does a page still say what a superseded rule said?** | `grep -l "^supersedes: [0-9]" raw/rules/` — for every rule that supersedes one, every page citing the old number is a finding |
| **Which pages has nothing linked to?** | Every page under `wiki/` except the index: `grep -rl "<path>"` over `wiki/`. No inbound link is a finding |
| **Which names have no page?** | Every switch, lamp, LED, display, coil, backlight channel, award, cue and state, read from the tracked inputs beside this checkout — gameplay.md §2 and §14, hardware.md §2–§6, a sound set's `sounds.json`, `MasterControlProcess::allStates()` — against every page's `aliases` and title. A name nobody claims is a rule nobody cut, or a page nobody wrote |
| **Does a sentence lack a rule behind it?** | Read every page for a sentence with no `[NNNN]` link. A `TBC`/`TBD`/`TODO` sentence is not a finding; a confident sentence with no citation is |
| **Is the index whole?** | Every page under `wiki/` has a line; every line names a page that exists; the summaries still describe the pages |
| **Which markers are open?** | `grep -rn "TBC\|TBD\|TODO" wiki/` — listed, not judged. This list is what the project gets out of the wiki: each is a rule nobody has written |

## Writing it down

- One line in `wiki/log.md`: `<when>  lint    N findings, M pages written`.
- The findings, in the reply, as a numbered list: the claim, the two pages or the name, the fix.
- A finding that is a page to write: write it, cite the rules, add it to the index.
- A finding that is a wrong page: fix the page, in the same pass, citing what it should have cited.
- A finding that is a wrong or missing *rule* is next door's — gameplay.md's, or a body's
  document — and is reported as a batch for the owner, never fixed from here.
- One commit: *lint: N findings, M pages*.

## What not to do

- Do not edit a rule file to resolve a contradiction. Add a rule, or report it.
- Do not quiet a finding by removing a page's claim; cite it or mark it `TBC`.
