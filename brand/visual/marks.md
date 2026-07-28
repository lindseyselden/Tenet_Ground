---
title: Marks
type: visual-marks
status: draft
updated: 2026-07-28
source: governance rules #01–#02; ground-ring.md (perforation logic, ground-truth line); decisions/2026-07-28-screen-surfaces.md
---

# Marks

The non-typographic graphic system: every element that is neither type nor photograph. This file
defines which marks exist, what each carries, and how variation encodes meaning.

Typography ([`typography.md`](typography.md)) governs letterforms. This governs geometry. Together
they are the whole of what Tenet Ground draws.

## What a mark is, and is not

> **A representational icon illustrates a concept. An encoded mark carries a value.**

A padlock is a picture of security. The Ground Ring's perforation pattern is a behavioral signature
rendered as geometry — change the signature and the pattern changes, because the pattern *is* the
signature. The first is forbidden ([`../anti-patterns.md`](../anti-patterns.md)); the second is native
to this brand and is its most distinctive visual property.

The operative test:

> **If the mark would look the same when the underlying value changed, it is decoration and has
> failed.**

## The governing principle

From [`ground-ring.md`](ground-ring.md), extended from the object to the page:

> **The system is uniform; the signature is individual.**

The *primitive* is locked and identical everywhere. The *variation within it* is the data. This is
the ring's locked-exterior / variable-interior logic applied to two dimensions, and it is why the
mark system can be small and still say a great deal.

## The four primitives

Every mark in the system is one of four. **No fifth primitive is added.** New meaning is made by
varying an existing primitive, never by inventing a shape.

### 1. The point

A filled square. The atom of the system — a single discrete value or state.

- **Square, not circle.** The brand is orthogonal institutional, not biomorphic
  ([`../decisions/forms.md`](../decisions/forms.md)). The circle is reserved for the ring and for the
  radial field.
- **Filled** = actual, observed, settled. **Outlined** = pending, projected, in verification.
- Carries state through color ([`color.md`](color.md)).
- The canonical instance is the status screen's state mark.

### 2. The line

A hairline. Registration, division, or relation.

- **Registration:** marks a datum — the Ground Ring's engraved gold "ground-truth line" is the
  canonical instance.
- **Division:** separates fields, as on a divided status-screen plane.
- **Relation:** connects a point to what it refers to.
- One weight. A second weight is a new primitive; use position or length instead.

### 3. The field

An array of points whose **density carries magnitude or variance**.

- The canonical instance is the Ground Ring's interior perforation pattern: constellation-sparse for a
  calm baseline, dense and uniform for high cognitive-load tolerance.
- Density is the variable. Point size stays constant within a field.
- A field is always bounded — it has an edge, and the edge means something.
- This is the primary primitive of the **evidence register**.

### 4. The radial

Concentric bands about a centre. Encodes **depth of verification** — how far out from the human body
a question sits.

- **Radius selects the band; the band is the signal.** The five verification signals nest from the
  body outward: Ground Pulse, Execution Field, Operating Envelope, Intent Vector, Mutual Ground. See
  [`../lexicon.md`](../lexicon.md).
- **Band thickness is the tolerance range** for that signal. A point's position across the thickness
  is its deviation; a point crossing a boundary is a breach.
- **Angle encodes time** across the verification window.
- The centre is always the transaction under examination. Nothing else occupies it.
- Concentric boundaries are lines (primitive 2), not decoration.
- **Points are never connected into a polygon.** Connecting them produces a radar chart, the
  category's most exhausted data-visualization cliché. Points stay discrete against the density field.
- The radial is the one place circular geometry is permitted — it encodes a nested structure rather
  than softening a form, and it is the same geometry as the Ground Ring read from above.

## How meaning is carried

**A mark varies in one dimension at a time.** Position, density, size, or fill — never two at once. A
mark carrying two variables carries neither legibly, and is the most common route back to decoration.

| Variable | Encodes |
| --- | --- |
| **Position** | Identity, time, or category |
| **Density** | Magnitude, variance, confidence |
| **Size** | Reserved. Not used to encode; scale belongs to type |
| **Fill** | Actual vs. pending |
| **Colour** | State only — see [`color.md`](color.md) |

Size is deliberately withheld. If everything can grow, hierarchy stops meaning anything, and the
surface becomes a dashboard.

## Colour

State semantics only, per [`color.md`](color.md) — chartreuse verified, amber anomaly, editorial red
not viable. A mark is never coloured for emphasis, grouping, or variety.

All marks **flat, bounded, fully opaque**, on transparent or opaque grounds alike. The substrate may
be transparent; the mark may not
([`../decisions/2026-07-28-screen-surfaces.md`](../decisions/2026-07-28-screen-surfaces.md)).

Accent limits from `color.md` apply: no accent exceeds ~10% of the frame.

## Composition

- Marks sit on the same grid as type. They are not placed optically.
- A field and a radial may occupy the same composition; **two radials may not** — the centre is
  singular, as the subject is.
- Marks never overlap. Occlusion implies depth, and depth is forbidden
  ([`../governance-rules.md`](../governance-rules.md) Rule #01).
- Where a mark and type compete for the same position, type yields. The mark is the measurement; the
  type labels it.

## Forbidden

- **Representational pictograms** — padlock, shield, checkmark, brain, globe, any picture of a concept
- **A fifth primitive.** If a new meaning needs carrying, vary an existing mark
- Marks whose appearance would not change if the underlying value changed
- Gradient, glow, transparency, or blur on any mark
- Outline weights other than the single hairline
- Overlap, drop shadow, or any implied z-depth
- Colour used for grouping, emphasis, or variety rather than state
- Size used as an encoding variable
- Two variables encoded in one mark

## Canonical instances

| Instance | Primitive | What it encodes | Source |
| --- | --- | --- | --- |
| Ring perforation pattern | Field | The wearer's behavioural signature | [`ground-ring.md`](ground-ring.md) |
| Ground-truth line | Line (registration) | The datum; role or seniority by count | [`ground-ring.md`](ground-ring.md) |
| Amber indicator | Point | Operational state | [`ground-ring.md`](ground-ring.md) |
| Status-screen state mark | Point | Verified / anomaly / not viable | [`../surfaces/status-screen.md`](../surfaces/status-screen.md) |
| Ground Hall receptacle grid | Field | One system, one intent — uniformity as specification | [`ground-hall.md`](ground-hall.md) |

The first three predate this file. The system was already operating; this names it.

## Open items

1. **Field density needs a defined range.** Sparse-to-dense is currently qualitative. It needs
   endpoints, so two fields drawn a month apart are comparable.
3. **Does the point have a minimum size?** Below a certain scale a filled square reads as a dot and
   the orthogonal logic is lost.
4. **The Ground Mark is unspecified.** The buyer-facing certification mark
   ([`../audience.md`](../audience.md)) will need to be built from these primitives, or explicitly
   exempted as a logotype-class asset.

## Related

- Letterforms: [`typography.md`](typography.md)
- State colour: [`color.md`](color.md)
- The rules every mark answers to: [`../governance-rules.md`](../governance-rules.md)
- What marks are refused: [`../anti-patterns.md`](../anti-patterns.md)
