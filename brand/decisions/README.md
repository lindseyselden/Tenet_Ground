# brand/decisions/ — the evolution log

The brand is **not static**. Whenever a canonical `brand/` file changes meaningfully, a dated record
is added here. This is an **append-only audit trail** — add new entries, never rewrite old ones. The
`brand-evolver` skill produces a record (with the proposed edits) for you to save here; you can also
write one by hand.

This log was **seeded from the original drift analysis** — the failures and resolutions surfaced
while building the scaffold are the brand's founding decisions.

## File naming

`YYYY-MM-DD-short-slug.md`. If two land the same day, add a numeric suffix (`-2`).

## Record format

\`\`\`markdown
---
title: Short statement of the decision
type: decision
date: YYYY-MM-DD
status: active
changes:
  - brand/<file>.md
supersedes: null   # or the slug of an earlier decision this overrides
---

## What changed
One or two sentences on the concrete edit(s).

## Why
The reasoning or trigger.

## What this supersedes
Any earlier decision or wording this replaces (or "nothing — new direction").
\`\`\`
