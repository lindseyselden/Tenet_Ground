---
title: Status Screen
type: surface
surface: status-screen
status: draft
updated: 2026-07-28
source: A5 UI/brand system WIP; governance rules #01–#04; decisions/2026-07-28-screen-surfaces.md
---

# Status Screen

The standing verification surface in Tenet Ground environments — the free-standing transparent plane
on which the system's ground truth is legible. This file is the fidelity source for the surface: what
is **authored**, what may be **generated**, and how the two are combined. It is checked against
[`../governance-rules.md`](../governance-rules.md) like any other asset.

Unlike [`../visual/ground-ring.md`](../visual/ground-ring.md) and
[`../visual/ground-hall.md`](../visual/ground-hall.md), which specify *things*, this file specifies a
**surface**. Its brand-carrying properties are grid, type, density, and state — not material and
light. That distinction governs everything below, and is the reason this file exists.

## What it is

A frameless transparent plane, held clear of a wall, carrying the live state of the ground truth
layer. It is an **environmental instrument, not a personal dashboard**: it reports the state of the
system, and any Architect passing it reads the same thing. There is no login, no personalization, no
notification.

It answers one question at a glance — *is intent verified* — and rewards a second, longer look with
the audit detail beneath. Glanceable and interrogable, in that order.

Permitted by Rule #01 under the four free-standing conditions. It is not the Ground Hall's
flush-mounted signage and elevator type system; that remains a separate, opaque, wall-set surface.

## Register

From [`../voice.md`](../voice.md), narrowed to this surface.

- **Values, not sentences.** The surface states; it does not narrate. `INTENT VERIFIED`, not
  "Everything looks good!"
- **Labels are nouns.** Never instructions, never questions. No verbs addressed to the reader.
- **No reassurance.** "All systems normal" is a warm failure. The steady state is stated flatly and
  then left alone.
- **No urgency.** An anomaly is reported at the same volume as a verification. Severity is carried by
  color and position, never by exclamation, size jump, or motion.
- **The lexicon is used as fact.** `BEHAVIORAL WHITELIST`, `HFD`, `GROUND TRUTH` appear unexplained.
  See [`../lexicon.md`](../lexicon.md).

## Grid & structure

The plane is a **12-column × 8-row modular field**. All divisions land on module boundaries; nothing
is optically placed.

- **Margin:** minimum one column on all four sides. The field never runs to the plane's edge.
- **Negative space:** ~40% of the plane stays empty, per Rule #03. This is the same breathing the
  architecture gets, applied to data.
- **Comparison** divides the field on column boundaries only — halves (6 / 6) or thirds (4 / 4 / 4).
  **Maximum three simultaneous views.** A fourth is an array.
- **Divisions are marked by a single hairline rule**, full height of the field. No gutters wide enough
  to read as separate panels, no boxes, no cards, no containers. The plane stays one plane.
- **One assertion per view.** In a divided plane, each view carries exactly one.

## Type

Three faces, three jobs. No face does another's work.
See [`../visual/typography.md`](../visual/typography.md).

| Face | Role on this surface |
| --- | --- |
| **IBM Plex Mono** | Every numeric value, identifier, timestamp, and status token. The data voice. |
| **IBM Plex Sans** | Labels, field names, wayfinding. The infrastructure voice. |
| **Newsreader** | The human register. At most one line per plane — and only when there is something human to say. |

### Scale

Three steps, per typography.md's "the asserted value is monumental; the audit detail is precise
beneath it."

| Step | Role | Relative size |
| --- | --- | --- |
| **Assertion** | The single monumental value or state | `1.0` |
| **Register** | Supporting values — up to five | `0.30` |
| **Audit** | The detail rows beneath | `0.15` |

The jump from Assertion to Register is deliberately large. A shallow scale reads as a dashboard; a
steep one reads as a monument with an audit trail, which is the brand thesis made typographic.

Rule #04 governs: **if you notice the typeface before you read the value, the type has failed.**

## Data density

- **One assertion.** Never two.
- **Up to five registers.** Beyond five, the surface is a dashboard and has failed.
- **Audit rows are unbounded** but live in a single bounded field, set in Mono at the audit step.
  Length is fine; sprawl is not.
- Nothing on the plane is decorative. Every mark carries a value or labels one.

## Color application

Ground is the architecture itself, seen through the plane. Marks are matte black on light
architecture, off-white on dark. From [`../visual/color.md`](../visual/color.md):

| Token | Meaning on this surface |
| --- | --- |
| **Chartreuse / acid green** | Verified. Live signal. The steady state. |
| **Warm amber** | Anomaly. Matches the Ground Ring's status semantics exactly. |
| **Editorial red** | Not viable. Terminal state, alert lines. |
| **Mustard** | Reserved for editorial/data emphasis; not a state. |

All marks **flat, bounded, fully opaque** — per the substrate/color distinction in `color.md`. The
plane is transparent. Nothing drawn on it is.

Accents stay ≤10% of the surface.

## States

| State | Behavior |
| --- | --- |
| **Dormant** | No data. The plane reads as clear glass and the space returns to architecture. The default before arrival and after departure. |
| **Verifying** | In progress. Carried by an incrementing Mono counter — motion is *data*, never decoration. No spinner, no pulse, no progress bar. |
| **Verified** | Steady. Chartreuse. Stated once and left alone. |
| **Anomaly** | Amber. Position and color change; size and volume do not. |
| **Not viable** | Editorial red. The terminal state — the transaction the system is architecturally incapable of processing. |

State changes are transitions that **carry**, not transitions that perform. A change preserves the
identity of the value that changed, so the eye can follow it from one state to the next — a hard cut
loses that, and legibility with it. Duration is bounded by the Zero-Lag Standard
([`../beliefs.md`](../beliefs.md)): a transition that outlasts the thing it reports has failed. No
easing that dramatizes, no celebratory motion on verification, no idle loops.

*(The full temporal register — duration, easing, what may move and why — belongs in a canonical
`visual/motion.md`. Until that file exists, this paragraph governs.)*

## Governance

How each rule lands specifically here.

- **Rule #01 — Technology Presence.** The plane must satisfy all four free-standing conditions:
  transparent, frameless, singular in view, non-emissive. The architecture must read before the data.
- **Rule #02 — Color Behavior.** The severe test on this surface. Every mark flat, bounded, opaque.
  No gradient fills, no area charts with fades, no glow behind the plane, no translucent overlays.
- **Rule #03 — Compositional Authority.** ~40% negative space. The field is presented, not
  aggrandized. No centered hero number floating in a void.
- **Rule #04 — Typographic Neutrality.** Value before typeface. Neutral faces only; the logotype does
  not appear on this surface.

## Forbidden

Surface-specific failure modes, beyond the anti-territories in
[`../anti-patterns.md`](../anti-patterns.md):

- Cards, rounded containers, drop shadows, any implied z-depth
- Gradient fills, area charts with fades, translucent data marks
- Glow or bloom behind or around the plane
- Motion that does not carry a value — spinners, decorative easing, celebratory transitions, idle loops
- **Representational pictograms** — padlock, shield, checkmark-as-reassurance, any picture standing in
  for a concept. Encoded geometric marks are permitted and native to the brand: a representational
  icon *illustrates* a concept; an encoded mark *carries* a value, the way the Ground Ring's
  perforation pattern carries a signature. *(The mark system belongs in a canonical
  `visual/marks.md`; until it exists, this distinction governs.)*
- Dark-mode-with-neon conventions
- More than three simultaneous views
- The logotype anywhere on the surface

## Generated vs. authored

**The load-bearing section, and the reason this file is structured differently from the object specs.**

An image model's brand-carrying competence is material and light. The Ground Ring and the Ground Hall
locked well because those *are* their brand-carrying properties. A surface's are grid, type scale,
density, hierarchy, and state — none of which a model can hold. Prompting for a status screen returns
a photograph of a screen-shaped object with rendering where the design decisions should be.

| Layer | Source | Why |
| --- | --- | --- |
| Grid, type scale, hierarchy | **Authored** | Not material properties. No model holds them. |
| Data content and state logic | **Authored** | Semantic. Must be true to the system. |
| Color assignment to state | **Authored** | Meaning, not appearance. |
| Division and comparison rules | **Authored** | Compositional logic. |
| The plane's physical presence | **Generated** | Material, optics, edge, how light meets glass. |
| The architecture behind it | **Generated** | Fully in the model's competence. |
| Lighting, siting, environment | **Generated** | Same. |

### The workflow rule

> **A model may render the plane. It may not compose what is on it.**
>
> Any published image of a status screen in situ is a **composite**: an authored artboard placed into
> a generated environment. It is never a single generation.

This is not a limitation to apologize for. It is the correct division of labor, and stating it
explicitly is what makes the system defensible: the machine builds the world, the designer authors the
system, and the seam between them is declared rather than hidden.

## Open items

Design calls that are yours, not mine. Each is flagged because the spec has to assert *something* and
I would rather you overrule a stated position than fill a blank.

1. **Newsreader on this surface — present or absent?** I have permitted one line, to carry the
   "numbers have nerves" register. The stricter reading is that a verification surface has nothing
   human to say and Newsreader never appears here. Both are defensible; the second is more austere.
2. **The one-accent-per-composition rule needs a surface-level exception.** `color.md` defaults to one
   accent per composition, but a status screen showing verified *and* anomaly simultaneously is doing
   its job. Proposal: on this surface the rule becomes **one accent per state**, not per composition.
   If you agree, it wants its own short decision record.
3. **Scale ratios (1 / 0.30 / 0.15) are a starting proposal**, not a derived system. Set them against
   a real render and a real reading distance, then fix them here.
4. **Divisions marked by a hairline rule** — confirm against a comparison layout. If the rule reads as
   a border, drop it and let the grid do the work with space alone.
5. **Grid dimensions (12 × 8)** assume a landscape plane. If the canonical plane is portrait or
   square, this needs restating.
6. **Motion and marks are governed inline here as a stopgap.** Both are world-level concerns, not
   surface-level ones. When `visual/motion.md` and `visual/marks.md` exist, the two paragraphs in
   **States** and **Forbidden** shorten to pointers.
