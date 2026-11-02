# Patchwork Quilt

The canonical home of **git.pp** and **stitch** — the two halves of one thesis about many agents working as one: git.pp derives *what the state is* from an append-only record, and stitch accounts for *who may change it, within what budget, provably*.

- **git.pp** — a Git substrate for many agents working one codebase at once, where the task is the atom, state is derived from an append-only record, and provenance is the arbiter.
- **stitch** — a tiny, language-portable substrate primitive for accountable agent state: eleven verbs (attest, delegate, contest, revoke…) over a signed, hash-chained ledger, with a conservation law that budgets how much any agent may change the world per tick. Four implementations — Python, Rust, C99, and a Lean 4 formalisation in which minting soundness and the conservation bound are machine-proven.

A patchwork quilt is pieces that stand alone, joined by visible seams into something that works as one thing. That is the design: every task is its own patch (its own repository), the seams are the record, and the whole stays inspectable — any patch can be lifted out, examined, or replaced without unpicking the rest.

## The family

- **git.pp-ng** — the substrate: Worker + Artifacts implementation, the fold, the conformance corpus, the runner. For anyone who wants the semantics and the corpus that pins them, before the tooling.
- **gitpp-action** — the fold inside your own CI: derived state as a job summary, from one workflow step, calling no external service. For teams who want the derivation with nothing new to trust.
- **gitpp-app** — the GitHub App: the same fold, posting the derived state as a Check on every push. It reads your contents and writes nothing but Checks. For teams who want the Check natively, without CI plumbing.
- **git.pp-desk** — the captain's desk: a projection of the record (burn it, rebuild it from the record alone, get the same answer). For anyone who wants to watch the record decide, step by step.
- **git.pp-grid** — the shared grid: defaults that stand until changed, proposals as visible bids, per-seat renderings of one record. For teams who coordinate by standing defaults rather than fresh claims.
- **gitpp-beam** — the fold on the BEAM (Elixir): a conformance spike that proved the semantics on a second runtime against the corpus. It predates the retraction law — that port is owed there, declared in the open, not hidden. For anyone who wants the semantics proven on a second runtime.
- **stitch** — a tiny portable primitive for accountable agent state: 11 verbs, a conservation law, a hash-chained JSONL ledger, and Ed25519 attestations — one spec held to four implementations (Python, Rust, C99, and a Lean 4 formalisation in which minting soundness and the conservation bound are machine-proven). For builders who need state changes to carry accountability.
- **stitch-dogfood** — the family's public evidence for stitch: a live booking board kept as a stitch ledger that anyone can audit end-to-end. For anyone who wants to check the claim instead of trusting it.

The org's ninth public repository is **.github** — this profile.

Developed in the open under SuperInstance; the products live here now. The evidence lives in the open too: stitch-dogfood, listed above, is kept here because the audit *is* the product claim — and git.pp's dogfood repos ([gitpp-demo-quilt](https://github.com/SuperInstance/gitpp-demo-quilt), [gitpp-dogfood-day1](https://github.com/SuperInstance/gitpp-dogfood-day1), [gitpp-dogfood-b1](https://github.com/SuperInstance/gitpp-dogfood-b1)) stay under SuperInstance, next to the workshop that runs them.

## The arrangement

[SuperInstance](https://github.com/SuperInstance) is the forest — the open-development sketchbook where things are figured out, with the full history of how they were discovered. Patchwork Quilt is the garden — the finished, public-facing form. Development happens there; graduated work lives here.
