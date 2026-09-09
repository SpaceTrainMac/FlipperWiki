# FlipperWiki

```
        what does that lamp mean?
        what just happened?
        what do I do now?
```

**This repository has prose of its own, and it is the only one in the project that does.** It is a
wiki for whoever is at the glass of the Space Train (MAC, 1987) — the cabinet, the
[Visual Pinball table](../FlipperVPX) or the [browser simulator](../FlipperSimulator) — one page per
thing a player can point at, written and kept by an LLM. Nothing under `wiki/` is written by a
person. What a person does is **add the next rule**, ask questions, and read.

**It is built the way Karpathy's LLM Wiki is built.** Three layers: the raw sources, which here are
**the rules of the game, one file each, added one at a time**; the wiki the LLM compiles from them;
and the schema, [CLAUDE.md](CLAUDE.md), which says how. Three operations — ingest, query, lint — and
a fourth this project needed, cut. The reasoning, and what was decided against, is
[docs/concepts/open/20260909-a-wiki-for-whoever-is-at-the-glass.md](docs/concepts/open/20260909-a-wiki-for-whoever-is-at-the-glass.md).

## Adding a rule

**Write one file under `raw/rules/`, numbered after the last, in the shape
[CLAUDE.md](CLAUDE.md#a-rule-file) gives — or ask a session to cut a section of a document into
rules**, which is the `wiki-cut` skill. Then ask it to ingest the rule: it reads it, tells you what
it took from it, writes the pages, updates the index and the log, and commits. Say *no* to a
takeaway before the commit and the pages change; that is the cheapest correction the wiki will ever
get.

**A rule is never edited.** When the machine changes, add a new rule that says so and names the one
it supersedes. Lint finds the pages that still say the old thing.

**What you saw is a rule too.** An evening at any glass goes into `raw/observations/`, dated and
naming the body, and is ingested the same way; where it disagrees with a rule, the page shows both
and decides nothing.

## Asking

Open a session on the folder holding the checkouts, with the skills linked
(`../FlipperArchitecture/link_skills.sh`), and ask. The answer comes from the pages with citations;
one that needed more than one page is filed under `wiki/questions/`.

## Reading

`wiki/index.md` is every page, one line each. Any markdown reader works; Obsidian opened on
`wiki/` works too, because links are relative paths.

## Which way the arrows point

**This repository reads nothing and is read by nothing.** Every rule names the document it was cut
from, which is a citation and not a dependency: the wiki answers from its own pages. It is the
second root in [structure.md](../FlipperArchitecture/structure.md)'s map — **once it has a row
there**, which waits on the remote under the organisation. Until then it is a local checkout, and
the root's link checks do not read it.

## What is here

| | |
|---|---|
| [`CLAUDE.md`](CLAUDE.md) | The schema — for the LLM |
| [`raw/rules/`](raw/rules/README.md) | The rules, one file each, verbatim with provenance. Never edited |
| [`raw/observations/`](raw/observations/README.md) | What a person saw at which glass. Never edited |
| `wiki/` | The pages, the index and the log. Written by the LLM only |
| [`.claude/skills/`](.claude/skills/) | `wiki-cut`, `wiki-ingest`, `wiki-query`, `wiki-lint` |
| [`docs/concepts/`](docs/concepts/README.md) | The dated design records |

## Licence

The **SpaceTrain Dialectical Public License v1.0** ([LICENSE.md](../FlipperEngine/LICENSE.md)),
like the rest of the project.
