---
title: Colour is specified — two palettes, and colour means state
type: decision
date: 2026-07-28
status: active
changes:
  - brand/visual/color.md
  - brand/visual/logo.md
supersedes: null
---

## What changed

`color.md` is rewritten. Four things follow from it.

**1. There are two palettes, and they are not interchangeable.**

- **Palette A — the rendered world.** Material and light, specified in words, no values. Matte black
  PVD, raw concrete, gold-as-matter, amber-2700K-as-light, the editorial accent set the scaffold
  points at. A rendered surface has a range, not a value; hex here would be false precision.
- **Palette B — the authored surfaces.** Exact values, because a drawn surface has one. Ink `#171717`,
  Paper `#F5F5F5`, Card `#FFFFFF`, Grey `#D2D1D7`, Held `#F7D04A`, Not viable `#E93526`,
  Field `#D6F4EA`.

The behaviour rule — flat, bounded, editorial; never gradient, glow, atmosphere — binds both, unchanged.

**2. Verification carries no colour.** The verified state is the default and does not announce itself.
Only exceptions are marked.

**3. Colour is state, never grouping.** Dimensions, categories and sections are distinguished by name,
position and scale. An earlier working version of the verdict surface assigned one colour per
verification signal; it was withdrawn.

**4. Field is not code.** In the evidence register, data has not yet been read and carries no assigned
meaning — colour there is compositional field, and `Field` mint is its value. In the verdict register
everything means something and only state colours appear. No colour does both jobs on one surface.

**The logotype is Ink or Paper on authored surfaces**, never gold; gold fill on the mark belongs to
the rendered world. The optional gold hairline accent is removed from `logo.md`.

## Why

**On specifying values at all.** `color.md` described colour in words — "chartreuse / acid green — live
data, verified signals" — and words do not constrain a rendering engine or a drawing tool. Whatever
the tool produced became the palette by default, on every asset, and the only correction available was
by eye. The palette was never authored; it accumulated. Palette B's values were sampled from work
already made and judged good, which makes the specification a record of a decision rather than a new
constraint.

**On the split.** Two colour systems had been operating inside one file: colour as a property of
material and light, which an image model reads, and colour as a specified value carrying a specified
meaning, which a designer draws. They have different units and different failure modes, and merging
them is why the file could not hold values. The split follows the same line as
`surfaces/README.md` — the model builds the world; the designer authors the system.

**On verification carrying no colour.** `beliefs.md` and `voice.md` both hold that the brand does not
announce, and that an anomaly is reported at the same volume as a verification. A palette in which the
default state is unmarked and only exceptions are coloured is that principle made operational. It also
produces more force, not less: on a surface where four values are achromatic, the one that is not is
unmissable.

**On colour as state rather than grouping.** A colour assigned to a category would look identical if
the underlying value changed, which is the explicit failure test in `marks.md`. Category colour is
decoration wearing a system's clothes.

**On field and code.** The evidence register shows data before it has been read; the verdict register
shows what reading produced. Colour that is compositional in the first and semantic in the second is
not an inconsistency — it is the distinction the two registers exist to make. **Meaning is assigned by
the act of reading, which is what verification is.** The consequence is that the evidence-to-verdict
transition is field resolving into code: unassigned colour locking into state. The transition
therefore carries information rather than decorating one, satisfying the motion rule in
`surfaces/status-screen.md`.

## What this supersedes

Replaces `color.md` wholesale. Nothing in Palette A is lost — the dominants, the gold/amber
matter-and-light distinction, the amber exception, and the scaffold's editorial accent tokens all
survive, now scoped to rendered assets.

Amends `logo.md`: the colour rule is scoped by surface class, and the optional gold hairline accent is
removed. `logo.md`'s existing forbidden treatments stand — flat gold *fill* is permitted in the
rendered world; gold as a *finish* (foil, gilding, metallic shine) remains forbidden.

The substrate-transparency clause from `2026-07-28-screen-surfaces.md` carries over unchanged.
