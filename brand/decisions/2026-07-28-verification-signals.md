---
title: The five verification signals, and the concentric encoding they produce
type: decision
date: 2026-07-28
status: active
changes:
  - brand/lexicon.md
  - brand/visual/marks.md
supersedes: null
---

## What changed

**Five verification signals are named.** The Behavioral Whitelist's "rhythmic pulse" is now specified
as five measurable signals, each answering a distinct question about whether a transaction's
originating world is real:

| Domain | Signal | Question |
| --- | --- | --- |
| Human | **Ground Pulse** | Is the person real? |
| Machine | **Execution Field** | Is the environment real? |
| Organization | **Operating Envelope** | Is the operation real? |
| Purpose | **Intent Vector** | Is the intent real? |
| Relationship | **Mutual Ground** | Is the shared context real? |

Full definitions in [`lexicon.md`](../lexicon.md).

**The evidence layer's geometry is fixed as concentric, not angular.** Radius selects the band; the
band is the signal. Band thickness is the tolerance range, a point's position across that thickness is
its deviation, and a point crossing a boundary is a breach. Angle encodes time across the verification
window. Points are never connected into a polygon.

This closes `marks.md` open item #1.

## Why

**On the signals.** The set was generated wide and then filtered against a single hard test: *could a
Digital Twin with the target's complete observable behavioral history reproduce a passing value?* Any
signal that survives observation-based replication is worthless by construction, because the adversary
in this world is defined as a perfect replica of observable history.

The five survivors cluster where they should — in what cannot be observed from outside: a living
body's state, a real computational environment, an operation's actual boundary, forward intent rather
than past behavior, and knowledge that exists only *between* two parties. None of them is a feature of
the transaction. Each is a feature of the world the transaction came from. That is what separates this
from anomaly detection with better branding.

**Mutual Ground** was named last and deliberately. The working name, *Shared Memory*, is a literal
computing term and read as engineering rather than as institutional vocabulary. Mutual Ground names
the concept and the geometry at once: the outermost band is the perimeter held in common, and it is
the only signal that requires both parties to exist at all.

**On the geometry.** Five signals plotted as angular sectors with points extending outward is a spider
chart — the most exhausted form in data visualization, and a direct route into the
"hyper-stylized generic" territory [`anti-patterns.md`](../anti-patterns.md) refuses.

The correction came from the signals themselves. Human → Machine → Organization → Purpose →
Relationship is not a list; it is a nesting, expanding from a single body outward to the space between
two organizations. Each domain contains the one before it. Drawing them as concentric bands is the
honest reading of the structure rather than a stylistic preference.

Two consequences follow, both load-bearing:

- **The verdict becomes visibly derived.** A breach is a line being crossed, not a state asserted.
  This is brand principle #4 — "our AI is not a black box; the logic of every stop must be auditable" —
  made drawable rather than claimed.
- **The evidence layer has the same geometry as the instrument.** Concentric bands around a human
  centre is a Ground Ring read from above, and the innermost band is exactly what the ring's
  perforated interior reads off the body. The visualization and the object are the same form at
  different scales.

## What this supersedes

Nothing — this is new vocabulary and a first encoding.

It closes `marks.md` open item #1 (the radial's encoding) and amends primitive 4 from an
angular-sector reading to the concentric one.

`ground-ring.md` is unaffected but is now doubly canonical: its perforation logic was the first
instance of a density field, and its concentric section is the first instance of the radial.
