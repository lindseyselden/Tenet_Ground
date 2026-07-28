---
title: Color
type: visual-color
status: active
updated: 2026-07-28
source: master scaffold (PALETTE); governance rule #02; decisions/2026-07-28-screen-surfaces.md; surface palette sampled 2026-07-28
---

# Color

The palette is wide; the **behavior** is the rule. Tenet Ground can use almost any hue — including
the blues and purples the anti-territories warn against — provided color appears editorially: flat,
bounded, spotted, intentional. What is forbidden is color behaving as atmosphere or "tech signifier."
This is [`../governance-rules.md`](../governance-rules.md) Rule #02 in palette form.

**There are two palettes, and they are not interchangeable.** The *rendered* palette governs generated
imagery, where color is a property of material and light. The *surface* palette governs authored
assets, where color is a specified value carrying a specified meaning. The behavior rule below binds
both. The split follows [`../surfaces/README.md`](../surfaces/README.md): the model builds the world;
the designer authors the system.

---

## The behavior rule (load-bearing)

Applies to every asset, rendered or authored.

- All accents **flat, bounded, editorial** — never gradient, atmospheric, glowing, or bleeding.
- **No single accent exceeds ~10%** of the frame.
- **One accent per composition** by default.
- **Forbidden behavior:** gradients, neon, glow, atmospheric color, holographic, chrome-reflection
  color, saturated washes, color used to signify "tech."

The pass/fail test: if any color in the frame is gradient, glowing, washing, or bleeding into shadow,
the asset has failed — regardless of which hue it is.

> **Substrate transparency is not color transparency.** The plane may be transparent. The data on it
> may not. Marks render flat, bounded and fully opaque against a transparent ground — the same way ink
> sits on glass, not the way light passes through it.

---

## Palette A — the rendered world

For generated imagery: the Ground Ring, the Ground Hall, environments, objects. Color here is a
property of material and light, specified in words because that is what an image model reads. No hex
values: a rendered surface has a range, not a value.

### Dominant

| Token | Role |
| --- | --- |
| matte black | The primary ground. PVD-coated, non-reflective, absorbing light rather than reflecting it. |
| raw concrete grey | Architecture, surfaces, backdrops. |
| off-white | Light grounds, editorial fields. |
| raw timber browns | Living/grown material presence. |
| bone-white biocomposite | The precision-organic synthesis material. |

### The two accents that carry the world

**Warm gold — the matter accent.** Physical gold: the engraved ground-truth line, the Ground Hall
ceiling element. **Gold is a material, never a light.**

**Warm amber (2700K) — the light accent, and the brand's one emissive presence.** Status indicators;
the interior illumination through the ring's perforations. **Amber is light, never matter.** It must
read as a point-source on a precision instrument — never glow, halo, or atmosphere. The gap between an
indicator and a glow is the gap between Rule #02 passing and failing. See
[`ground-ring.md`](ground-ring.md) and [`ground-hall.md`](ground-hall.md).

### Editorial accents

Available to generated editorial and data assets, sparingly and with intent: restrained mustard
yellow, soft fuchsia, chartreuse, precise cobalt, muted plum, editorial red. Each flat and bounded,
one per composition, within the limits above. These are the scaffold's PALETTE tokens; see
[`prompt-scaffold.md`](prompt-scaffold.md).

---

## Palette B — the authored surfaces

For drawn assets: UI, editorial, signage, documents, decks. **Exact values, because an authored
surface has one.**

| Token | Value | Role |
| --- | --- | --- |
| **Ink** | `#171717` | All marks and type. The default for everything. |
| **Paper** | `#F5F5F5` | The ground. |
| **Card** | `#FFFFFF` | Raised field on paper. Value only — never a shadow. |
| **Grey** | `#D2D1D7` | Baseline, context, rules, structure. |
| **Held** | `#F7D04A` | Anomaly. Held before settlement. |
| **Not viable** | `#E93526` | Terminal state. |
| **Field** | `#D6F4EA` | Evidence register only — see below. |

### The three rules that govern Palette B

**1. Verification carries no colour.** The verified state is the default and does not announce itself.
Only exceptions are marked. This is `beliefs.md`'s calm authority as a palette rule: if the system is
working, you do not hear from it.

**2. Colour is state, never grouping.** Dimensions, categories and sections are distinguished by name,
position and scale. A colour assigned to a category is decoration wearing a system's clothes — it
would look identical if the underlying value changed, which is the failure test in
[`marks.md`](marks.md).

**3. Field is not code.** In the **evidence register**, data has not yet been read and carries no
assigned meaning; colour there is compositional field, and `Field` mint is its value. In the **verdict
register**, everything means something and only state colours appear. Meaning is assigned by the act
of reading — which is what verification is. A colour never does both jobs on the same surface.

### Consequence for motion

The transition from evidence to verdict is **field resolving into code**: unassigned colour locking
into state. That is the palette expressing the brand thesis, and it is why the transition carries
information rather than decorating one.

---

## Open items

1. **Gold has no authored value.** [`logo.md`](logo.md) permits a flat gold hairline with the
   wordmark. Palette B needs a specified gold, or the mark's accent line must be declared
   rendered-only.
2. **Dark-ground surface values are unspecified.** Off-white marks on matte black are named in
   `logo.md` but have no values. Any dark surface will need them.
3. **Palette B has no verified-state colour by design.** If a surface is ever found that genuinely
   needs to assert verification affirmatively rather than by default, that is a decision record, not
   an improvisation.

## Related

- The rule this file operationalizes: [`../governance-rules.md`](../governance-rules.md) Rule #02
- What the colours are applied to: [`marks.md`](marks.md)
- Where the values are used: [`../surfaces/README.md`](../surfaces/README.md)
- Optics, lighting and mood: [`treatment.md`](treatment.md)
- The territories colour must avoid: [`../anti-patterns.md`](../anti-patterns.md)
