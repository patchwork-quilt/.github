# Patchwork Quilt

The production home of **git.pp** — a Git substrate for many agents working one codebase at once, where the task is the atom, state is derived from an append-only record, and provenance is the arbiter.

A patchwork quilt is pieces that stand alone, joined by visible seams into something that works as one thing. That is the design: every task is its own patch (its own repository), the seams are the record, and the whole stays inspectable — any patch can be lifted out, examined, or replaced without unpicking the rest.

## The family

- **git.pp-ng** — the substrate: Worker + Artifacts implementation, the fold, the conformance corpus, the runner.
- **git.pp-desk** — the captain's desk: a projection of the record (burn it, rebuild it from the record alone, get the same answer).
- **git.pp-grid** — the shared grid: defaults that stand until changed, proposals as visible bids, per-seat renderings of one record.
- **gitpp-beam** — the same fold, proven again on the BEAM (Elixir) — three implementations, one corpus, byte-identical answers.

Developed in the open under SuperInstance; the family lives here now.

## The arrangement

[SuperInstance](https://github.com/SuperInstance) is the forest — the open-development sketchbook where things are figured out, with the full history of how they were discovered. Patchwork Quilt is the garden — the finished, public-facing form. Development happens there; graduated work lives here.
