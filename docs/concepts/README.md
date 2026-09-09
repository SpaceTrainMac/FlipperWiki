# Concepts

Dated design records for **the wiki — its raw layer, its pages, and the four operations that
maintain them**.

Each file is a snapshot of the reasoning behind one decision, frozen at the point the decision was
made — the alternatives that were rejected and why, the arithmetic behind the constants, and the
traps that would not show up as a failing test.

Not live documents. Once something is built the tree is authoritative for *what* it does. These keep
the *why*.

**Naming:** `YYYYMMDD-topic.md`, date first so each directory sorts chronologically. The date is when
the design was settled, not when it was implemented.

**Which directory a file sits in is its status:**

| Directory | Holds | Maintained |
|---|---|---|
| [open/](open/) | designed, not built yet — the work in progress | **yes.** Fix what you find wrong, in place |
| [done/](done/) | designed and built | no |
| [declined/](declined/) | designed and decided against | no |

`done/` and `declined/` are an archive position. A file that has landed in either is frozen as it was
written. A file leaves `open/` when the last step of its implementation plan is done, or when the
decision goes the other way, and it is not rewritten on the way out.

## open/

| Document | Covers |
|---|---|
| [20260909-a-wiki-for-whoever-is-at-the-glass.md](open/20260909-a-wiki-for-whoever-is-at-the-glass.md) | **The record this repository was built from, and the first one in it.** Settled at the root on 2026-09-09 and moved here the day the repository was created, as the bridge record moved to FlipperVPX; its *What this is* keeps both sides. Why the raw unit is one rule, verbatim, appended and never edited (§2); what *processed by an LLM* means, the gist's five outputs per rule (§3); where the rules come from and in which order (§4); the four skills, `index.md` and `log.md` kept as the gist has them (§6); why a twelfth repository, confirmed by the owner (§12); and §14, the first version's three inventions with why each lost. |

## done/

*Empty.*

## declined/

*Empty.*

---

**Which repository a record belongs to** is the deletion test in
[FlipperArchitecture/README.md](../../../FlipperArchitecture/README.md) — *would this still be true
if every line of the Raspberry Pi software were deleted tomorrow?* — and its companion, *would every
repository that has one of these have to agree on it?* A decision about this wiki's own shape
belongs here; one about the machine belongs in `FlipperArchitecture/docs/`.
