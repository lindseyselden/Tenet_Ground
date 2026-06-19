---
title: Specify behavior, not presence — for matte and for light
type: decision
date: 2026-06-04
status: active
changes:
  - brand/visual/ground-ring.md
  - brand/visual/color.md
  - brand/visual/treatment.md
supersedes: null
---

## What changed
Material and light tokens now specify *behavior*, not just presence. "Matte black" became
"PVD-coated, non-reflective, absorbing light not reflecting it." The amber indicator was constrained
to a discrete exterior point with interior illumination and tunneling effects explicitly forbidden.

## Why
Two drifts had the same root cause. (1) "Matte black surgical steel" rendered with specular
reflections — the model's default for "premium black product" is polished, and the word "matte"
names a property without saying what it does. (2) The amber indicator rendered as atmospheric halo
spilling onto the plinth, violating Rule #02. Naming a thing does not constrain how it acts; specify
what the property *does*.

## What this supersedes
Nothing — establishes the "behavior over presence" principle now reflected in the ring spec and the
color behavior rule.
