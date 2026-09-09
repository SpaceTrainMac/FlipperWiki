# A wiki for whoever is at the glass

**Settled 2026-09-09. Not built.** A knowledge base for the person standing at the machine — the
cabinet in the flat, the Visual Pinball table, or the browser simulator — built the way Andrej
Karpathy's **LLM Wiki** is built: **the rules of the game are added to it one at a time, as raw
sources, and an LLM processes each one** — reads it, says what it took from it, writes or updates
the pages it touches, updates the index, and logs what it did. Nothing in the wiki is written by a
person; what a person does is add the next rule, ask questions, and read.

**Revised the same evening, on the owner's correction, and the first version is kept in
[§14](#14--what-the-first-version-said-and-why-it-lost).** The first version read the project's
documents in place, invented a per-page hash witness against five checkouts and a lint script to
recompute it, and refused the pattern's own `log.md`. The correction was three sentences — *google
llm-wiki. I want the rules be added one by one to the llmwiki. to be processed by an LLM.* — and it
turns the design the right way round: **the raw layer is the rules, one file each, appended and
never edited**, and the LLM's work is the ingest of each rule, exactly as the gist describes it. The
witness and the script go, because a raw source that lives inside the wiki has nothing outside to
drift from.

**Three bodies, one game, one wiki.** *The table* in the request that opened this record is
unspecified between the real one and the simulated one, and that is the design: the rules are the
engine's and are the same at all three glasses, so a rule is one raw file and `HOUSE_BALL` is one
page; what differs between the bodies is a handful of rules of their own, marked with the body
([§7](#7-w7--three-bodies-one-game-and-what-differs-is-a-rule-marked-with-the-body)).

**Step 1 of the plan was run on 2026-09-09, and on the builder's reading it passed; the owner's
reading is pending.** Two rules of gameplay.md §3 — *`M` and `C` pay for as long as `A` is left
alone*, then *`A` opens a 20-second window* — were cut by hand and ingested by hand, and the second
rewrote the M-A-C page's `A` paragraph to hold both claims and added one cycle sentence citing
both, rather than appending a second summary. One page, not two stapled. The repository was created
locally the same evening, and this record moved into it.

**It lives in a twelfth repository, `FlipperWiki`**
([§12](#12-w12--a-twelfth-repository-and-why-none-of-the-eleven-can-hold-it)), because it has prose
of its own and owns no fact — the shape FlipperHandbooks has, one rule inverted.

## What this is

A dated design record, in the shape [docs/concepts/README.md](../README.md) describes: the reasoning
at the moment it was worked out, kept so the alternatives that lost stay lost for a stated reason.

**Settled here, at the root, on the second question in
[README.md](../../../../FlipperArchitecture/docs/../../FlipperArchitecture/README.md#what-belongs-in-here-and-the-two-questions-that-decide-it)**: the
wiki adds a twelfth row to [repositories.json](../../../../FlipperArchitecture/docs/../../FlipperArchitecture/repositories.json) and rewrites
`structure.md` in every checkout, and a design that changes the map cannot be settled inside one
square of it — [20260830-project-review.md](../../../../FlipperArchitecture/docs/concepts/open/20260830-project-review.md) is the same argument for a
review. **It moves to `FlipperWiki/docs/concepts/open/` on the day that repository exists**, as
[20260904-a-ball-on-the-playfield.md](../../../../FlipperVPX/docs/concepts/done/20260904-a-ball-on-the-playfield.md)
was settled here and moved to FlipperVPX the day it was created, with both sides kept in this
paragraph. **Moved here on 2026-09-09, the evening the repository was created locally** — before its row in
`repositories.json`, which waits on the remote — so that `open/` means maintained in place by
whoever is building it. The index row at the root now says *(moved)* and points here.

**It is authoritative for the shape of the wiki and for nothing the wiki says.** What the machine
does is [gameplay.md](../../../../FlipperArchitecture/docs/gameplay.md); what the 1987 machine did is
[machine.md §1](../../../../FlipperArchitecture/docs/machine.md#1-the-game-as-the-machine-tells-it); what each body does that a
cabinet would not is that body's own document. A rule file in the wiki is a copy of one of those
with its provenance on it, and a page that disagrees with the rules it cites is wrong.

**The numbers are `W`**, on the rule FlipperVPX's records follow — the letter says what kind of
thing a decision decides. A `D` is about the machine. **A `W` is about a description of the machine
written for a reader at the glass**, which is a different kind of thing because it can be wrong in a
way that makes a player try something the machine does not do — the argument
[player-card.md](../../../../FlipperArchitecture/docs/player-card.md) makes for a card of its own rather than the 1987 one.

**The pattern** is
[Karpathy's gist](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f), created
2026-04-04. Three layers: *raw sources*, immutable, that the LLM reads and never edits; *the wiki*,
LLM-generated markdown the LLM owns entirely; *the schema*, a document — his is `CLAUDE.md` — that
*"tells the LLM how the wiki is structured, what the conventions are, and what workflows to
follow."* Three operations. **Ingest**: *"the LLM reads the source, discusses key takeaways with
you, writes a summary page in the wiki, updates the index, updates relevant entity and concept pages
across the wiki, and appends an entry to the log."* **Query**: *"the LLM searches for relevant
pages, reads them, and synthesizes an answer with citations."* **Lint**: *"periodically, ask the LLM
to health-check the wiki. Look for: contradictions between pages, stale claims that newer sources
have superseded, orphan pages with no inbound links."* Two files hold it together: `index.md`, *"a
content-oriented catalog organized by category"* that *"the LLM updates on every ingest"*, and
`log.md`, *"an append-only record of what happened and when."* And the division of labour, which is
the sentence this record is built to honour: *"You're in charge of sourcing, exploration, and asking
the right questions. The LLM does all the grunt work — the summarizing, cross-referencing, filing,
and bookkeeping."*

---

## 1. W1 — The reader is at the glass, and *observes* is two readers

**The reader has a flipper button under each hand, or is standing beside somebody who does.** Not
the operator, whose document is [cabinet.md](../../../../FlipperEngine/docs/cabinet.md) and whose
question is *why does it show `E 102`*; not the developer, whose question is *which class raises
that*. The question at the glass is one of three: *what does that mean*, *what just happened*, *what
do I do now*. Three documents in this project were written for that reader —
[player-card.md](../../../../FlipperArchitecture/docs/player-card.md), 324 words;
[how-to-play-pinball.md](../../../../FlipperArchitecture/docs/how-to-play-pinball.md), about no machine in particular; and
[gameplay.md](../../../../FlipperArchitecture/docs/gameplay.md), *what SPACE TRAIN does, from in front of the glass*, 11 056 words
in fourteen sections ordered by mechanism — and none of them is ordered by what a player is looking
at.

**A player is looking at a lamp, not at a mechanism.** `HOUSE_BALL` blinking is answered in
gameplay.md §12, the lamp's address in [hardware.md](../../../../FlipperArchitecture/docs/hardware.md), the sound that plays when
it stops in [sound.md §4](../../../../FlipperEngine/docs/sound.md#4-the-catalogue), and what the
flyer said about it in [machine.md](../../../../FlipperArchitecture/docs/machine.md). Four documents, three repositories, one
question. The wiki is where they meet on one page, and the page exists because four rules that
mention that lamp were each ingested and each one touched it.

**"Observes" names two readers, and both are in scope.** The spectator beside the player, who sees
the backbox go dark for the bonus count and wants to know whether the machine is broken — it is
counting, for about 43 seconds
([using-the-table.md §5](../../../../FlipperVPX/docs/using-the-table.md#5--what-it-does-that-a-cabinet-would-not));
and the person reading what the machine wrote down afterwards — the state log, the high score file,
the odometer — which every body keeps
([using-the-table.md §3](../../../../FlipperVPX/docs/using-the-table.md#3--the-machines-own-files)).
What those files mean is a handful of rules like any other, and the files themselves are never
ingested ([§13](#13-w13--what-was-watched-is-a-rule-too-and-what-the-machine-wrote-is-not)).

| The reader | Their document today | Verdict |
|---|---|---|
| The operator at the service menu | cabinet.md, [states/setup.md](../../../../FlipperEngine/docs/states/setup.md) | **out** — a second wiki, when it is asked for |
| The developer | everything else | **out**, same reason |
| The player | the card, the manual, gameplay.md | **in** |
| The spectator | nothing — the card assumes the buttons | **in** |
| The reader of the machine's own files | four documents in two checkouts | **in**, as rules about what the files say |

## 2. W2 — A rule is the raw unit, and it is added one at a time

**One rule is one file under `raw/rules/`, and it is the only kind of raw source the wiki has apart
from an observation.** A rule is a statement of what the machine does that a player could act on:
*the `M` and `C` lanes pay 30 000 each, again and again*; *a drain within fifteen seconds of
`OUTFIRE` hands the ball back*; *`BALL IN PLAY` counts turns down*. It is appended, numbered, and
never edited. When the machine changes, a new rule is added that says so and names the one it
supersedes, and lint finds the pages that still say the old thing — which is the gist's *stale
claims that newer sources have superseded*, made literal.

**The grain is gameplay.md's own unit, the bold-led paragraph, and the count decides it.** Every
paragraph in that document opens with a bold sentence that is the claim; that is the house rule for
every document here, and it makes the document already cut into rules. Counted 2026-09-09:

| Grain | Files | Words each | What one ingest touches |
|---|--:|--:|---|
| a section of gameplay.md | 14 | ≈ 800 | twenty pages; the takeaways discussion is a review of a chapter, which is not a review |
| **a bold-led paragraph** | **128** | **≈ 85** | **two to six pages; the takeaways fit in one screen and a person can say *no* to one** |
| an item on the player card | 12 | ≈ 25 | one page, and the card leaves out the `500` lanes and both flyer bonuses on purpose |

Of the 128, §2's 32 switch rows and §14's 29 award rows are tables rather than paragraphs and are
cut one row each, so the first pass is **about 190 rules** from one document — every switch, every
award, and every paragraph of §3 to §13. That is the number of ingests, not of sessions: a session
processes rules in sequence and commits after each, and a rule is a few minutes of an LLM's work.

**A rule file is the text verbatim and its provenance above it, nothing else.**

```markdown
---
rule: 0031
title: M and C pay 30 000, repeatably
source: FlipperArchitecture/docs/gameplay.md § 3. M-A-C
as-of: 1892207                # the commit of that checkout the text was copied from
body: game                    # game | cabinet | vpx | simulator | 1987
supersedes:                   # a rule number, when this one replaces an earlier one
---
**Two of the three pay when the word is complete.** …the paragraph, exactly as gameplay.md has it…
```

**Verbatim, on the rule this project learned on 2026-09-07: a source declared as truth is carried
whole**, and a paraphrase in the raw layer would be the LLM's first opinion disguised as a source.
`as-of` is the commit the text was copied from — a fact about the copy, not a witness that anything
recomputes. `body` is
[§7](#7-w7--three-bodies-one-game-and-what-differs-is-a-rule-marked-with-the-body)'s; `1987` is a
body of its own, because a rule from [machine.md](../../../../FlipperArchitecture/docs/machine.md) describes a machine that is not
under the glass and a page has to say so in the sentence.

**A person may write a rule too, and the header says so.** `source: RooL, at the cabinet,
2026-09-14` is a legal provenance. That is the case the owner's sentence is about — *the rules be
added one by one* — and the design does not privilege the document over the person: both are raw,
both are immutable, and where they disagree the wiki page shows both and decides nothing
([§13](#13-w13--what-was-watched-is-a-rule-too-and-what-the-machine-wrote-is-not)).

| Alternative | Verdict | Why it lost |
|---|---|---|
| Read gameplay.md in place, no copies — the first version | **No** | [§14](#14--what-the-first-version-said-and-why-it-lost): it needed a witness and a script to know when a page was behind, and it made the raw layer somebody else's document, which the pattern's whole point is that it is not |
| Ingest whole sections | **No** | the table above — twenty pages per ingest is not a thing a person reviews |
| Paraphrase the rule when copying | **No** | 2026-09-07's lesson, and a raw layer that is already an opinion cannot be linted against anything |
| Edit a rule file when the machine changes | **No** | the gist: raw is immutable. A new rule with `supersedes:` is what lint keys on |

## 3. W3 — Ingest is what the LLM does with one rule, and it is five outputs

**"Processed by an LLM" means the gist's ingest, applied to one rule, and it produces exactly five
things.** In the order the gist gives them:

| # | The gist says | Here |
|--:|---|---|
| 1 | *reads the source* | the rule file, and the pages its names already have |
| 2 | *discusses key takeaways with you* | three to eight lines: what the rule means at the glass, which names it touches, whether it contradicts a page. **This is the review**, and a person saying *no* here is the cheapest correction the wiki will ever get |
| 3 | *writes a summary page* | `wiki/rules/0031-m-and-c-pay-30000.md` — the rule at the glass, one paragraph, citing the raw file |
| 4 | *updates the index* and *relevant entity and concept pages* | `index.md`; the pages under `things/` for each lamp, switch, coil or display the rule names, under `moments/` for a ceremony or state it touches, under `rules/` for a concept it belongs to — M-A-C, the count, the hole bonuses |
| 5 | *appends an entry to the log* | one line in `log.md`: date, `ingest`, the rule number, the pages touched |

**One commit per rule, after the takeaways, and the commit subject is the log line.** The house
style — a lower-case sentence — *ingested rule 0031, M and C pay 30 000: four pages*. `log.md` and
`git log` then say the same thing, and that is deliberate: the gist's log is what an LLM reads at
the start of a session, and `git log` is what a person reads; neither can be forgotten because the
skill writes one and the commit is the other.

**The entity pages are where the compounding happens, and they are why one at a time is right.** A
page for `HOUSE_BALL` is written the first time a rule names that lamp and is *added to* by every
later rule that does; after 190 rules it says everything the machine does with it, in the order the
rules were ingested, each sentence citing its rule. Nothing decides in advance what the page will
contain; the rules decide it as they arrive. That is Karpathy's *persistent, compounding artifact*,
and it is the property a cut of gameplay.md can never have
([§5](#5-w5--the-wiki-is-compiled-not-cut-and-that-is-the-departure)).

**A page's front matter is four fields, and it was pinned by the readiness check rather than by the
design.** `title`, `type` — one of `rule`, `thing`, `moment`, `concept`, `body`, `question` —
`aliases`, the names the page claims for the lint count of
[§10](#10-w10--lint-is-the-llms-and-it-asks-the-gists-three-questions-and-one-more), and `body`.
Nothing else: the rules a page rests on are cited sentence by sentence in its text, by number, and
a `sources:` list in the front matter would be a second copy of those citations that lint would
have to reconcile. This is the one thing the record had left to the builder, and it is written
here so that the schema in `CLAUDE.md` copies it rather than decides it.

**The takeaways are spoken, not filed.** The gist's step 2 is a conversation; here it is the
session's reply before the commit, and it is not a file — a filed takeaway would be a second summary
page. What a person says back is what changes the pages before they are committed.

## 4. W4 — Where the rules come from, and in which order they are added

**gameplay.md first, top to bottom, because it is the authority and its order is already the
machine's.** [gameplay.md](../../../../FlipperArchitecture/docs/gameplay.md) is *the authority for what this machine does*; its
sections run from the quantities the machine tracks (§1) through every switch (§2), the mechanics
(§3–§9), the end of a ball, a turn and a game (§10–§12), what the glass shows (§13) and every award
in one table (§14). Cut into its paragraphs and rows, that is about 190 rules, added in document
order so that a rule about the count arrives after the rules about what feeds it.

| Batch | Source | Rules | `body` |
|---|---|--:|---|
| 1 | gameplay.md §1–§14, and its two closing sections | ≈ 190 | `game` |
| 2 | [machine.md §1](../../../../FlipperArchitecture/docs/machine.md#1-the-game-as-the-machine-tells-it) — the flyer's feature set, the rule card verbatim, the pricing card | ≈ 30 | `1987` |
| 3 | [using-the-table.md §4–§5](../../../../FlipperVPX/docs/using-the-table.md#4--playing-it) — the keys, the nudge, two balls, the drawn backbox | ≈ 15 | `vpx` |
| 4 | [using-the-simulator.md](../../../../FlipperSimulator/docs/using-the-simulator.md) §2, and [cabinet.md §1–§3](../../../../FlipperEngine/docs/cabinet.md#1-the-settings-file) where a setting shows at the glass | ≈ 20 | `simulator`, `cabinet` |
| 5 | [sound.md §4](../../../../FlipperEngine/docs/sound.md#4-the-catalogue) — which cue speaks when, one rule per cue | 43 | `game` |
| 6 | the state documents — [intro](../../../../FlipperEngine/docs/states/intro.md), player select, play, the draw, highscore, credits — where a paragraph says what the glass shows | ≈ 40 | `game` |
| 7 | what a person adds afterwards — rules of their own, and observations | open | any |

**Batch 1 is the whole of the first milestone, and it is enough to answer a player.** The card is
derived from gameplay.md alone and is judged sufficient to go under the glass; a wiki built from the
same document answers everything the card does, one page per thing, before any second source is
touched. Batches 2 to 6 are ordered by how often a player asks: what the flyer promised and the
machine does differently comes up at every first game; the keys come up once.

**The cutting is a person's act with an LLM's hands, and it is not an ingest.** Turning a section
into rule files is mechanical — one paragraph, one file, the header filled from where it was copied
— and the skill does it on request, a section at a time, *without* processing anything: the files
land in `raw/rules/` and the ingest of each is a separate, later step with its own takeaways. Two
steps rather than one, so that a person can look at the cut before the wiki is built from it.

## 5. W5 — The wiki is compiled, not cut, and that is the departure

**Every sentence in the five handbooks exists first in a document, and a wiki page has sentences
that exist first in the wiki.** That is the first paragraph of
[FlipperHandbooks' README](../../../../FlipperHandbooks/README.md), and it is why the books are a
*selection* — a corrected document becomes a corrected book without anybody rewriting anything. A
page about `HOUSE_BALL` is one paragraph compiled out of four rules from three documents, and no
manifest can cut that: the assembler keeps sections whole, so the book answers the question in four
places.

**So the wiki is a third kind of product, after the documents and the books**, and the project has
already accepted compiled prose once: [how-to-play-pinball.md](../../../../FlipperArchitecture/docs/how-to-play-pinball.md) *is
compiled, not measured*, and went into `docs/` and into print on 2026-09-09. The difference is that
here the sources are rules cut from this project's own documents, each carrying where it came from,
so every compiled sentence has a raw file to be checked against.

| Alternative | Verdict | Why it lost |
|---|---|---|
| A sixth handbook, cut by manifest | **No** | one lamp is four rules in three documents, and a cut keeps sections whole |
| Reorder gameplay.md by what a player looks at | **No** | gameplay.md is the specification `src/games/` is built toward; a second ordering is a second copy of the specification ([20260828-move-handbooks.md §1b](../../../../FlipperEngine/docs/concepts/done/20260828-move-handbooks.md#1b--the-walkthroughs-second-copy-of-the-book-and-what-it-cost)) |
| Retrieval over the documents at question time, no wiki | **No** | the gist's argument: an answer derived again every time is never fixed. A page is fixed once and cited afterwards |
| A generated stub per lamp from hardware.md, the LLM writing the rest | **No** | a fourth copy of hardware.md's tables; the page the reader wants is the paragraph, and the paragraph is what ingest writes |

## 6. W6 — Three layers as the gist has them, and the two files it names are kept

**`raw/`, `wiki/`, and a schema — and the schema is `CLAUDE.md`, as in the gist, with the three
operations as skills beside it.** In the engine's convention `CLAUDE.md` is *a map, not a rulebook*;
in the wiki it is the schema, because that is the file the pattern names and an LLM reads first. It
says what the layout is, what a rule file looks like, what an entity page looks like, and what the
three operations do — in a page, pointing at the skills for the workflow. The skills are
`.claude/skills/wiki-ingest`, `wiki-query` and `wiki-lint`, linked into the parent folder by
[link_skills.sh](../../../../FlipperArchitecture/docs/../../FlipperArchitecture/link_skills.sh), which is the only way a skill loads in a session opened
on the folder holding all twelve checkouts.

```
FlipperWiki/
  CLAUDE.md                  the schema - layout, conventions, the three workflows
  README.md                  for a person: what this is, how a rule is added, how to ask
  .claude/skills/
    wiki-cut/SKILL.md        one section of a document into rule files, no processing
    wiki-ingest/SKILL.md     one rule: read, takeaways, summary page, entity pages, index, log
    wiki-query/SKILL.md      answer from pages with citations; file the answer if it earned it
    wiki-lint/SKILL.md       contradictions, superseded claims, orphans, and the names with no page
  raw/
    rules/                   0001-….md …  one rule each, verbatim with provenance, never edited
    observations/            what a person saw at which glass, dated, never edited
  wiki/
    index.md                 every page, one line each, by category; updated on every ingest
    log.md                   append-only: date, operation, what was touched
    rules/                   one summary page per rule, the rule at the glass
    things/                  a lamp, a switch, a coil, a display, an LED, the backlight
    moments/                 attract, player select, the serve, the count, the draw, name entry, …
    concepts/                M-A-C, the bank, the count, the hole bonuses, the multipliers, …
    bodies/                  cabinet.md, vpx.md, simulator.md, 1987.md
    questions/               answers that were filed, dated
  docs/concepts/             this record, once the repository exists
```

**`index.md` and `log.md` are kept as the gist has them, and the first version was wrong to refuse
the log.** The gist's index is *content-oriented, organized by category*, updated by the LLM on
every ingest; its log is *append-only*, with a parseable timestamp per line. The first version
generated the index from front matter and dropped the log in favour of `git log`. Both refusals came
from this project's habit that a fact nobody can forget to update is the only kind that stays right
— and both miss that in this pattern **the LLM is the thing that cannot forget**: the ingest skill's
last two steps are the index and the log, and a skill that skipped them would be a skill that had
not run. What survives of the habit is one line in the lint skill — *does every page appear in the
index, and does every index line name a page* — which is a question an LLM answers by reading, not a
script.

**No `raw/` copy of a document that is not a rule.** The five checkouts beside the wiki are where
the documents live and where a rule's `source:` points; the wiki holds rules and observations and
nothing else in `raw/`. A whole document copied in would be the first version's mistake with an
extra step.

## 7. W7 — Three bodies, one game, and what differs is a rule marked with the body

**A rule is about the game unless its header says which body it is about.** The cabinet, the VPX
table and the browser simulator run one engine — *one engine, three deployments* is the owner's own
framing — so the 190 rules of batch 1 are `body: game` and `HOUSE_BALL` is one page. What differs is
short and each difference has a document already, and each becomes a rule of its own:

| Body | Its rules come from | What they say |
|---|---|---|
| The cabinet | cabinet.md, the card | the nudge and the tilt are the cabinet's own wiring and the host is never told; the plunger is a lever; the buttons drive the flipper coils in hardware |
| The VPX table | [using-the-table.md §4–5](../../../../FlipperVPX/docs/using-the-table.md#4--playing-it) | the keys; VPX's own nudge and tilt, which the engine sees as a drain; multiball is two balls; the backbox is drawn; the 43-second ceremonies with no ball in your hand |
| The browser simulator | [using-the-simulator.md](../../../../FlipperSimulator/docs/using-the-simulator.md) | no ball at all — a switch is a click; the page shows what the engine did, which is the *observer's* body |
| 1987 | [machine.md §1](../../../../FlipperArchitecture/docs/machine.md#1-the-game-as-the-machine-tells-it) | what the flyer advertised and the card said, which is not the machine under the glass and is what every first-time player has read |

**An entity page carries a body's rule as one sentence under the body's name, and the body page
carries the paragraph.** `TILT` on the backbox says *at the VPX table the tilt is VPX's own* and
points at `bodies/vpx.md`; the argument is there, once. That is what the `body:` field is for at
ingest time: the skill files a `vpx` rule's summary on the body page and touches the entity pages
with a line, not a paragraph.

## 8. W8 — Links are paths, never wikilinks, and the root checks the wiki for free

**Karpathy links with `[[page]]`, and here that would be a link no check can see.**
[check_anchors.py](../../../../FlipperArchitecture/docs/../../FlipperArchitecture/check_anchors.py) finds a link with one regular expression — line 76,
square brackets then parentheses — and [check_links.py](../../../../FlipperArchitecture/docs/../../FlipperArchitecture/check_links.py) with the same one; both take their
checkout list from [repositories.json](../../../../FlipperArchitecture/docs/../../FlipperArchitecture/repositories.json). A wikilink is invisible to both.
**The twelfth row is what turns them on for the wiki**, and from that day every link between pages
and every `source:` path in a rule file that is also written as a link is checked for existing, file
and anchor, by a tool nobody here maintains twice. Obsidian reads markdown links as well as
wikilinks, so the viewer loses nothing.

**The rule is [README.md's *Every link is a path*](../../../../FlipperArchitecture/docs/../../FlipperArchitecture/README.md#every-link-is-a-path)**, which
the wiki inherits by doing nothing: a citation is a path into the checkout beside, never a URL. A
page cites a rule file by path (`../../raw/rules/0031-….md`); a rule file cites its document by path
in `source:` and again as a link in its first line, so the anchor is checked.

## 9. W9 — A page says what its rules say, and where no rule answers it says so

**A page never states a rule that no raw file states.** The failure this guards against is the one
nothing mechanical can see: a plausible sentence the LLM wrote between two cited ones. So every
sentence on an entity page cites a rule by number, a `1987` rule is quoted with *1987* in the
sentence, and a body's rule with the body. **A sentence with no rule behind it is a lint finding**,
and it is the first thing the lint skill reads for.

**Where a player's question has no rule, the page carries the marker and lint lists it.** The
engine's [docs/README.md](../../../../FlipperEngine/docs/README.md#conventions) has three: `TODO`
for input no source can recover, `TBD` for a decision not taken, `TBC` for a fact only the machine
can confirm. *TBC — no rule says whether the knocker's third hit lands before or after the transfer*
is a better page than one that describes it. **That list is what the project gets out of the wiki**
beyond the reader: the gist's lint asks *what pages does the wiki lack*, and here the answer is
*which rule nobody has written*, asked by the only reader who has not been asking. A missing rule is
a finding for [gameplay.md](../../../../FlipperArchitecture/docs/gameplay.md), filed the way the engine's `defect` skill files
things left unfixed — as a batch next door, because that document is in a checkout the wiki may not
edit.

## 10. W10 — Lint is the LLM's, and it asks the gist's three questions and one more

**No lint script.** The first version wrote one; the correction is *to be processed by an LLM*, and
the gist's lint is a question put to the LLM — *health-check the wiki*. What a script would have
decided is either the root's already (links and anchors, once the row exists) or a thing an LLM
reads for in a minute (every page in the index). The lint skill asks:

| Question | From |
|---|---|
| do two pages contradict each other | the gist |
| does a page still say what a rule that has been superseded said | the gist — `supersedes:` in the rule header is what it keys on |
| which pages has nothing linked to | the gist |
| **which names have no page** — every switch, lamp, LED, display, coil, backlight channel, award, cue and state | this record: the tracked inputs know the names, and a lamp with no page is a rule nobody cut |
| does a sentence lack a rule behind it | [§9](#9-w9--a-page-says-what-its-rules-say-and-where-no-rule-answers-it-says-so) |
| is every page in the index, and every index line a page | [§6](#6-w6--three-layers-as-the-gist-has-them-and-the-two-files-it-names-are-kept) |

The names, counted 2026-09-09 from the tracked inputs: 32 switches
([gameplay.md §2](../../../../FlipperArchitecture/docs/gameplay.md#2-every-switch-and-what-closing-it-does)), 48 playfield lamps,
17 indicator LED addresses — 16 named and 180 *unmapped*, which is the first `TBC` a page will
carry — five six-digit displays and the status row, 9 coils and 3 backlight channels
([hardware.md](../../../../FlipperArchitecture/docs/hardware.md)), 29 awards
([gameplay.md §14](../../../../FlipperArchitecture/docs/gameplay.md#14-every-award-in-one-table)), 40 `sfx` and 3 `music` cues (any
set's `sounds.json`, [8-bit's](../../../../FlipperSounds/8-bit/sounds.json)), 14 top-level states —
**about 200 names**, and a page claims one in its `aliases:` line. A lint pass writes its findings
into `log.md` and, where a finding is a page to write, writes the page.

**Nothing gates, and that is not a loss.** The root's two checks gate links; everything else is a
lint finding an LLM writes down and a person reads. The first version had a coverage number that
turned into a gate at 100 %; this one has the same number as a line in the lint output, which is
what it was for.

## 11. W11 — A query answers from pages first, and a filed answer cites pages, never rules

**A question is answered from the wiki, and from the rule files only where the wiki is silent.**
That is the pattern's reason to exist — an answer built from the raw layer every time never improves
the wiki. **An answer is filed under `questions/` when it needed more than one page to give**: a
question answered by one page is a link to it; one that joined three is a synthesis the next asker
should not redo. A filed answer cites pages and never rules, so that it goes stale exactly when the
pages do and no faster. The asker is at a keyboard, in a session opened on the folder holding the
checkouts, with `wiki-query` loaded; a phone at the cabinet is a different product and is in
*Deliberately not here*.

## 12. W12 — A twelfth repository, and why none of the eleven can hold it

**Confirmed by the owner on 2026-09-09 — *ack. a twelfth repository* — after asking why**, and the
answer that settled it is the short form of this section: a repository is the unit that carries one
rule, one owner and one history, and the wiki fits none of the eleven.

**Each of the four places it could go breaks a rule that repository's README states in its first
paragraph.** Re-argued under the revision, because the revised wiki reads no checkout at build time
— its raw layer is its own — and one of the four arguments changed.

| Candidate | The rule it breaks | Verdict |
|---|---|---|
| **FlipperArchitecture** | `docs/` holds *facts the software does not get to overrule*, and *this is not an attic*. Two hundred LLM-written pages beside the archive would be read as archive, and every one of them is a paragraph *about* facts rather than a fact. The first version's objection — the root consumes nothing and this reads five — no longer applies, and this one does | **No** |
| **FlipperHandbooks** | *None of them has prose of its own* — the first sentence of [its README](../../../../FlipperHandbooks/README.md). A wiki is prose of its own and nothing else | **No** |
| **FlipperVPX** | one body of four | **No** |
| **FlipperEngine** | the handbooks were extracted from here at the cost of thirteen commits truncated to their handbook half ([20260828-move-handbooks.md §4](../../../../FlipperEngine/docs/concepts/done/20260828-move-handbooks.md#4--git-history-is-valuable-but-the-split-is-not-a-copy)); a product starts where it ends | **No** |
| **`FlipperWiki`, a twelfth** | owns no fact about the machine; its raw layer is copies with provenance; is read by none. The shape FlipperHandbooks has, one rule inverted | **Yes** |

**Its edges in [repositories.json](../../../../FlipperArchitecture/docs/../../FlipperArchitecture/repositories.json) are `reads: []`.** *Reads* is *what a
repository needs a checkout of in order to do its job, today*; the wiki's job is answering from its
own pages, and it needs no checkout for that. The five it was cut from are named in every rule's
`source:` line, which is a citation and not a dependency — the same distinction the root draws for
`FlipperMisc`. **That makes it the second root in the map**, beside FlipperArchitecture, and it is
the honest row: a `reads` written for the cutting step would be *an aspirational edge*, which
`repositories.json`'s own comment calls the one thing it cannot afford.

**The name follows FlipperHandbooks, named for its product.** *Wiki* occurs in two tracked
documents, both as somebody else's URL. **What the row costs**: when FlipperVPX arrived its row
moved *37 hand-typed sites in five checkouts*; a regex on 2026-09-09 finds **26 live sites in 22
files** that say *eleven* — 48 counting the frozen records, which are not repaired — plus twelve
`structure.md` copies and `overview.md`.

## 13. W13 — What was watched is a rule too, and what the machine wrote is not

**An observation is a raw source of the second kind, and it is ingested like a rule.** A person
plays an evening at a body and writes what they saw into `raw/observations/YYYYMMDD-<body>.md` —
*the count took longer than I expected; the knocker landed mid-transfer; the right `EXTRA BALL` was
lit and the saucer did not collect it*. Ingest reads it against the pages it touches, and where it
disagrees with a rule the page gains a **Watched** paragraph citing both. The rule's page is then
the one place where what was asserted and what was seen stand together, which is what
[gameplay.md's last section](../../../../FlipperArchitecture/docs/gameplay.md#what-nobody-has-watched) — *what nobody has watched*
— is asking for. **A discrepancy is not a correction**: the wiki has no authority over gameplay.md,
and a Watched paragraph is a finding with a citation at both ends, which is the form the `defect`
skill wants and *I think the count is slow* never has.

**The machine's own files are never ingested.** Every body writes `settings.json`, a high score file
and the odometer, and two bodies can write a state log. A wiki that copied a high score table would
be stale by the next game. What the files *mean* is a handful of rules — the fourteen state names
and why a game is one `intro -> play` line however many balls it took
([operations.md](../../../../FlipperEngine/docs/operations.md)); what the odometer's sixteen keys
count ([states/setup.md](../../../../FlipperEngine/docs/states/setup.md) under `STATISTICS`); what a
high score row is — and those are batch 4 and 6 of
[§4](#4-w4--where-the-rules-come-from-and-in-which-order-they-are-added).

## 14 — What the first version said, and why it lost

**Kept because the house rule is to correct in place and say so, and because each of the three
inventions will look reasonable again in a month.**

| The first version said | Why it looked right | Why it lost |
|---|---|---|
| **The raw layer is the five checkouts, read in place; nothing is copied** | one gameplay.md, one place to be wrong; *take a source whole* read as *do not copy it* | the pattern's raw layer is immutable *because it is the wiki's own*; a raw layer that is somebody else's live document is one the wiki cannot know it has fallen behind — which is what forced the next row |
| **Every page carries a `git hash-object` witness per source, recomputed by `lint.py` against five checkouts** | the project's answer wherever a thing cannot be gated: `check_drift.sh`, `vpx.origin`, `--dead` | it was solving a problem the revision does not have. A rule file never changes; a changed machine is a new rule with `supersedes:`; lint reads for the superseded claim. No hash, no script, no five checkouts at lint time |
| **No `log.md`; `index.md` generated from front matter** | *a fact nobody can forget to update is the only kind that stays right* | in this pattern the LLM is the thing that cannot forget — the log and the index are the last two steps of the ingest skill. The habit is right about scripts and wrong about a workflow whose executor is the same agent every time |
| **Twelve documents ingested, one commit each** | fewest ingests | *one by one* is the owner's sentence, and the table in [§2](#2-w2--a-rule-is-the-raw-unit-and-it-is-added-one-at-a-time) is why: a document's takeaways are a chapter and cannot be said *no* to; a rule's fit on a screen |
| **`reads:` the five checkouts** | `lint.py` needed them | `reads: []` — [§12](#12-w12--a-twelfth-repository-and-why-none-of-the-eleven-can-hold-it) |

**What survived unchanged**: the reader
([§1](#1-w1--the-reader-is-at-the-glass-and-observes-is-two-readers)), compiled-not-cut
([§5](#5-w5--the-wiki-is-compiled-not-cut-and-that-is-the-departure)), the bodies
([§7](#7-w7--three-bodies-one-game-and-what-differs-is-a-rule-marked-with-the-body)), markdown links
and the root's checks
([§8](#8-w8--links-are-paths-never-wikilinks-and-the-root-checks-the-wiki-for-free)), the citation
rule and the markers
([§9](#9-w9--a-page-says-what-its-rules-say-and-where-no-rule-answers-it-says-so)), the query
([§11](#11-w11--a-query-answers-from-pages-first-and-a-filed-answer-cites-pages-never-rules)), the
twelfth repository, observations, and the refusal to ingest the machine's files.

---

## What has to change first

**Everything in this table is in a checkout other than the one the wiki will be, and the wiki does
not exist yet.** Every row is a batch to be authorised, on the rule that has held since 2026-09-04,
and none of it is done by this record.

| # | Where | What | Why | Blocked |
|---|---|---|---|---|
| 1 | `FlipperWiki` | the repository, beside the eleven, with the remote under the organisation | nothing below has a place to land; a local `git init` is enough for every script here, which reads checkouts on disk | **the remote is the owner's** |
| 2 | [repositories.json](../../../../FlipperArchitecture/docs/../../FlipperArchitecture/repositories.json) | a twelfth row: `FlipperWiki`, *holds:* the wiki for whoever is at the glass — the rules of the game added one at a time as raw sources, and the pages an LLM compiles out of them; owns no fact about the machine; *reads:* nothing | turns `check_links.py`, `check_anchors.py` and `gen_structure.sh` on for the wiki | **FlipperArchitecture is read-only** |
| 3 | twelve checkouts | `./gen_structure.sh` after row 2; `overview.md` last and alone | generated, in the root's own order | as 2 |
| 4 | 26 live sites in 22 files | the hand-typed *eleven repositories* / *ten checkouts* — two each in `FlipperEngine/CLAUDE.md`, `conventions/README.md` and this repository's `implement-concept` skill, one each in eight FlipperVPX files, and the rest; measured by a regex on 2026-09-09 and re-taken the same evening for the readiness check, so the list is re-taken on the day | the eleventh row moved 37 | spans five checkouts |
| 5 | [README.md](../../../../FlipperArchitecture/docs/../../FlipperArchitecture/README.md#where-the-answers-are) | a row in *Where the answers are* — *What does that lamp mean, standing at the glass* → `../FlipperWiki` — and one sentence in the `docs/` row | a reader who lands at the root has to find the twelfth | as 2 |
| 6 | [gameplay.md](../../../../FlipperArchitecture/docs/gameplay.md#what-nobody-has-watched) | one sentence in *What nobody has watched*: where a watched thing is written down | that section is why `raw/observations/` exists | as 2 |
| 7 | [FlipperHandbooks' README](../../../../FlipperHandbooks/README.md) | one sentence: the product with prose of its own is next door | its first sentence is the rule the wiki inverts | **FlipperHandbooks is read-only** |
| 8 | `link_skills.sh` | nothing to edit; **run** once the wiki's four skills exist | a skill you cannot see is a skill that does not exist | a command, not an edit |

**Nothing in the engine has to change**, and that was checked rather than assumed: the odometer's
keys are live in [states/setup.md](../../../../FlipperEngine/docs/states/setup.md), the state log in
[operations.md](../../../../FlipperEngine/docs/operations.md).

## The implementation plan

**Step 1 could decline the design and needs no repository. Steps 2 and 3 build the wiki empty; 4 to
7 fill it one rule at a time; 8 is the row; 9 is the step nobody can shortcut; 10 is the
documentation; 11 is the generated files, last and alone.**

1. **One rule, by hand, end to end.** Cut one paragraph of
   [gameplay.md §3](../../../../FlipperArchitecture/docs/gameplay.md#3-m-a-c) — *`M` and `C` pay 30 000, repeatably* — into a rule
   file with the header of [§2](#2-w2--a-rule-is-the-raw-unit-and-it-is-added-one-at-a-time), in a
   scratch directory, and ingest it by hand: the takeaways, the summary page, the entity pages it
   touches (`30K_TOP_L`, `30K_TOP_R`, the `M` and `C` lanes, the M-A-C concept page), the index
   line, the log line. **Then a second rule that touches the same pages** — *`A` opens a 20 s window
   on the upper `EXTRA BALL`* — and see the pages compound rather than get rewritten. *Check:* a
   person reads the M-A-C page after the second ingest and says whether it is one page or two
   summaries stapled together. **Two summaries stapled declines this record**: the compounding is
   the whole value, and if the LLM cannot do it at two rules it will not at 190.
2. **The repository and the schema.** `FlipperWiki/` beside the eleven: `CLAUDE.md` as the schema,
   `README.md` for a person, the four skills, `raw/rules/` and `raw/observations/` with a README
   each stating *never edited*, an empty `wiki/` with `index.md` and `log.md` and its seven
   directories, and this record in `docs/concepts/open/`. *Check:* `./link_skills.sh --check` at the
   root reports four skills linked.
3. **The cut skill, on gameplay.md §3.** Ten rule files, headers filled, text verbatim, nothing
   processed. *Check:* `diff` of each file's body against the paragraph it came from is empty.
4. **Ingest the ten, one at a time, one commit each**, with the takeaways spoken before each commit.
   *Check:* `log.md` has ten lines, `index.md` names every page that exists, and the M-A-C concept
   page cites all ten.
5. **Cut and ingest the rest of batch 1**, section by section in document order — about 180 more
   rules. *Check:* the lint skill's names line reports no switch, lamp, LED, display, coil, award or
   state of the game without a page. Cues and bodies are still allowed to be missing.
6. **Batches 2 to 6**, in the order of
   [§4](#4-w4--where-the-rules-come-from-and-in-which-order-they-are-added). *Check:* the names line
   is empty, and every body page exists.
7. **A lint pass**, and its findings into `log.md`. *Check:* the pass writes at least the list of
   markers; a wiki with no `TBC` after 340 rules has not been read carefully.
8. **The twelfth row, and everything it moves** — rows 2 to 7 of the table above, as one authorised
   batch, in that order, `overview.md` last. *Check:* `./gen_structure.sh --check`,
   `./check_links.py`, `./check_anchors.py` — the last now reading the wiki — all clean.
9. **An evening at a glass, written down.** Somebody plays — the cabinet if RooL is standing at it,
   the VPX table otherwise — and writes `raw/observations/2026MMDD-<body>.md`: what was seen, in the
   order it was seen, with no reference to any page. Then it is ingested. **This machine cannot do
   it**, and the instruction is that directory's README from step 2. *Check:* at least one Watched
   paragraph exists, or the observation's last line says nothing disagreed.
10. **The documents.** The wiki's own README says what step 9 found; the root's README and
    gameplay.md carry rows 5 and 6; FlipperHandbooks' README carries row 7. **The handbooks: none of
    the five changes**, because no manifest names the wiki and the sentence added to that README is
    in no book — `../FlipperHandbooks/./build.sh --check` should say so.
11. **`./gen_overview.py`**, last and alone, at the root — the wiki is prose, and 340 rule files
    plus their pages will move the count by more than gameplay.md twice over.

## Deliberately not here

- **nashsu/llm_wiki, the desktop application** (https://github.com/nashsu/llm_wiki, v0.6.11 of
  2026-08-25, GPLv3). Considered on 2026-09-09, the evening this record was revised, and **declined
  by the owner: *the same concept — stick with your plan*.** It implements the same gist and would
  do the loop — a rule dropped into `raw/sources/` is watched, hashed, queued and ingested — but it
  brings its own fixed layout (`purpose.md`, `schema.md`, `entities/`, `concepts/`, `sources/`,
  `queries/`, `synthesis/`, `comparisons/`), writes `[[wikilinks]]` that the root's two checks
  cannot see, replaces the spoken takeaways of
  [§3](#3-w3--ingest-is-what-the-llm-does-with-one-rule-and-it-is-five-outputs) with an async
  review panel, and answers queries through its own search engine. What this project runs on is a
  session with skills loaded, and the record keeps the operations there. Reopening this means
  beating that sentence, not the feature list.
- **A hash witness, a lint script, a coverage gate** —
  [§14](#14--what-the-first-version-said-and-why-it-lost).
- **The session transcripts as a source.** Primary for *what did we decide*; the reader at the glass
  is not asking that; private, unversioned, 383 MB in the parent folder alone. A *why* a page wants
  is in the frozen records under `docs/concepts/done/` in three checkouts, and a rule may cite one.
- **Wikilinks** —
  [§8](#8-w8--links-are-paths-never-wikilinks-and-the-root-checks-the-wiki-for-free).
- **Ingesting whole documents, or paraphrasing a rule on the way in** —
  [§2](#2-w2--a-rule-is-the-raw-unit-and-it-is-added-one-at-a-time).
- **A generated stub per lamp, switch or coil** —
  [§5](#5-w5--the-wiki-is-compiled-not-cut-and-that-is-the-departure).
- **The operator's wiki and the developer's.** A second reader is a record of its own on the day it
  is asked for; nothing here forecloses it, and `things/` would serve both.
- **Retrieval, embeddings, a vector store.** The pattern replaces them, and the corpus is a few
  hundred rules.
- **Publishing it.**
  [20260819-going-public.md](../../../../FlipperEngine/docs/concepts/declined/20260819-going-public.md)
  declined publishing for the project, and every rule cites a private path.
- **A phone at the cabinet asking the wiki.** A product with a server in it; the simulator's page is
  the precedent for what a server on a cabinet costs to state honestly.
- **Printing it.** The card and the manual are the printed product for this reader
  ([STYLE.md](../../../../FlipperHandbooks/STYLE.md)).
- **Ingesting the machine's own files** —
  [§13](#13-w13--what-was-watched-is-a-rule-too-and-what-the-machine-wrote-is-not).
- **Editing any source from the wiki.** The arrow points one way, as it does for the handbooks; a
  rule that is wrong because its document is wrong is a finding next door and a new rule here.
