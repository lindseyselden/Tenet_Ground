---
title: Ground Ring
type: visual-subject
subject: ground-ring
status: active
updated: 2026-06-18
source: canonical Ground Ring product specification; brand-world description
---

# Ground Ring

The Integrity Architect's continuous biometric instrument, and the first canonical depicted product.
This file is the fidelity source: what is **locked** across every ring (the system) and what
**varies** per wearer (the signature). All ring renders — visual, marketing, editorial, future
evolutions — are checked against this file by `ring-fidelity-checker`.

## What it is

A matte-black, precision-machined band worn during all working hours, monitoring the wearer's own
behavioral baseline — cognitive load, decision fatigue, stress signature — during high-frequency
threat events. It reads ground truth from the body and treats the Architect's own behavioral
signature as evidence: a vendor may be deepfaked, but the Architect's pulse, focus, and cognitive
state can't be. By verifying the human in the loop, the ring closes the last gap in transactional
immunity.

## Locked across all rings (the System)

- **Form:** smooth cylindrical band exterior. No facets. No geometric breaks. No diamond-cut variants.
- **Finish:** matte black PVD coating. Fully diffuse. No reflectivity. The surface absorbs light, it
  doesn't reflect it.
- **Engraved line:** thin gold engraved line on the outer band — one or two parallel — registering
  the band horizontally. The "ground truth line."
- **Indicator:** a single discrete amber indicator inset on the exterior. Reads as a status indicator
  on a precision instrument, not as a feature.
- **Sensor strip:** a small precision-machined sensor or vent line on the outer band. Functional in
  appearance.
- **Interior surface:** finely perforated — the sensor face that meets the wearer. Never smooth,
  never decorative.
- **Interior illumination:** warm amber (2700K) visible *through* the perforations from interior
  sensors. Never spilling outside the perforations. Never atmospheric glow.
- **Proportion:** band height roughly equal to interior diameter. Substantial but unobtrusive.

## Calibrated per wearer (the Signature)

- **Interior perforation pattern:** density and arrangement vary per Architect — constellation-sparse
  for calm baselines, dense and uniform for high cognitive-load tolerance, directional or clustered
  for others. The biometric fingerprint translated into the sensor surface.
- **Cross-sectional profile:** subtle variation in how the band hugs the finger, calibrated to
  anatomy and the data-extraction needs of the role.
- **Gold-line count:** one or two parallel lines on the exterior — may indicate role, seniority, or
  specialization (to be defined).

## Forbidden in any ring

- Faceted or geometric exteriors (decorative form-making)
- Smooth or featureless interiors (loses the sensor logic)
- Multiple visible LEDs (single-indicator rule)
- Glossy or reflective exterior (PVD matte is non-negotiable)
- Glow, halo, or atmospheric light emanating from inside the ring
- Any interior pattern that reads as decorative rather than functional
- Consumer-tech signifiers: visible bezels, glass surfaces, branded logos, exposed connectors
- Crypto/luxury jewelry register: visible precious-metal mass, gem inset, ornamental engraving

## System logic

> **One system. One intent.** — the locked exterior, identical across every ring.
>
> **An intimate link between the human and the system.** — the variable interior, calibrated to each
> wearer.

The exterior speaks to the institution; the interior speaks to the individual. Both are present in
every ring, and the boundary between them must be visible.

## Status semantics

- **Steady warm amber indicator:** normal operation; behavioral baseline matches expected pattern.
- **Modulated rhythm:** anomaly detected; the modulation pattern conveys severity without text.
- **No screen, no notification text, no haptic alert visible to others.** The signal is legible to
  the wearer and to anyone nearby — auditability made visible.

## Rendering notes

Macro register: 100mm, raking-hard light, 4:5, plinth/vitrine implied (see
[`prompt-scaffold.md`](prompt-scaffold.md) and [`treatment.md`](treatment.md)). The recurring drift
is "matte black" rendering polished — specify behavior (PVD-coated, non-reflective, absorbing light)
not just the word "matte." The amber indicator must stay a discrete exterior point; forbid interior
illumination spilling onto the plinth (see `decisions/`).
