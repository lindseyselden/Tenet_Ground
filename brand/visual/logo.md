---
title: Logotype
type: visual-logo
status: active
updated: 2026-06-19
source: typographic extension; logotype adopted 2026-06-19
---

# Logotype

The wordmark, and the one place the visual system is licensed to assert. Everything else in the
type system is neutral by mandate (see `typography.md`); the logotype carries the single
signature. This file is the fidelity source for the mark — what is locked, how it is applied,
and the treatments that void it. It is checked against `../governance-rules.md` like any other
visual asset.

## What it is

TENET over GROUND — a two-line, all-caps, left-aligned wordmark in a heavy, high-contrast
sharp-serif. Stacked and squared, it reads as an orthogonal block: "one system, one intent"
made typographic.

## Why this face

A serif, so it rhymes with Newsreader — the "human" voice in the system — but its *own* face,
so the name carries a signature the body text does not. The distinctiveness is structural: it
comes from the letterforms themselves — the cut of the serifs, the contrast, the monumental
weight — not from any applied treatment. The serifs read scalpel-cut, which makes the mark
distinctive *through precision*: the clinical register rendered as type. The licensed
idiosyncrasy, earned the right way.

## Locked

- **Letterforms:** the adopted sharp-serif face (exact name to be confirmed — see Open items).
  No substitution with a system face.
- **Case & structure:** all caps, stacked two lines, left-aligned.
- **Distinctiveness is structural, never applied.** The mark is distinctive because of how it
  is *drawn*, not how it is *finished*. This is the governing principle; the forbidden list
  below is its consequence.
- **Color:** flat, single-color. Matte black on light grounds; off-white on dark grounds.
  Gold only as the brand permits — flat, as matter, never as a finish on the letterforms
  (see `color.md`).

## Variants

- `logo.svg` — black, primary, for light grounds.
- `logo-reversed.svg` — off-white, for matte black / dark grounds.
- Same outlined lockup; only the fill changes. No other recoloring.

## Application

- **Physical surfaces:** the mark is *engraved* — blind deboss, or flush flat ink — never
  raised, never foiled. This is the brand's own mark-making logic: the ring's engraved
  ground-truth line, the board-formed concrete of the Ground Hall. A debossed mark read by
  raking light is the canonical physical application.
- **Digital surfaces:** flat single-color, full opacity, no effects.
- **Optional accent:** a single flat gold hairline (the ground-truth line, see
  `ground-ring.md`) may sit with the mark — one line, flat, within the limits in `color.md`.
  Never on the letterforms themselves.

## Forbidden treatments

The render's failure modes, named so they don't recur. All follow from the "structural, not
applied" principle and from Rule #02 (`../governance-rules.md`); the anti-territories live in
`../anti-patterns.md`.

- Gloss, sheen, specular highlight on the mark or its ground
- Bevel, extrusion, drop shadow, any dimensional rise
- Gold foil, gilding, metallic shine — gold as costume rather than a flat mark
- Gradient, glow, halo, atmospheric light
- Diagonal, tilted, or dramatic placement; the mark sits orthogonal and level

## Clear space & minimum size (proposed)

- **Clear space:** cap-height of the mark on all four sides, minimum.
- **Minimum size:** GROUND no smaller than legible reproduction allows — roughly 15mm wide in
  print, 120px digital — below which the serif detail closes up. Confirm against final outlines.

## Files

- **Vector masters live in-repo** as text: `logo.svg`, `logo-reversed.svg`, here in
  `brand/visual/`. SVG is text, so it diffs and renders on GitHub — the logo is the standing
  exception to the media-outside-the-repo rule (see `../decisions/`).
- **Raster exports** (PNG at sizes, favicon, social) are binaries: they live in the external
  `assets/` library, indexed in `manifest.json`, generated from the masters. Not committed.

## Open items

- Identify the exact typeface, for accurate outlines and a complete spec.
- Finalize the lockup: track TENET out to GROUND's right edge for a closed rectangle, or keep
  it ragged right. Decide rather than inherit.
- Outline the type to paths and place `logo.svg` / `logo-reversed.svg`.
