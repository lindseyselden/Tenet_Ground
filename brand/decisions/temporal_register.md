---
title: Temporal register is the scaffold's weakest seam — flag now, tokenize later
type: decision
date: 2026-06-04
status: active
changes:
  - brand/visual/prompt-scaffold.md
supersedes: null
---

## What changed
The scaffold carries an explicit "known weak seam" note: era is encoded implicitly through materials
and named references, so text-only generation drifts toward present-moment register. Interim fix is
an explicit temporal token on the SUBJECT line; a standing TEMPORAL token is on the backlog for v2.

## Why
With image references removed, pure text produced a "warm and current" register rather than
2035-speculative. The scaffold had no explicit future-fluent token; temporal register is the
system's weakest layer.

## What this supersedes
Nothing — documents the open weakness rather than hiding it, per the principle that productive drift
is data, not failure.
