---
title: Master Prompt Scaffold
type: visual-scaffold
status: active
updated: 2026-06-18
source: master prompt scaffold (consolidated)
---

# Master Prompt Scaffold

The visual scaffold for generating brand assets with AI image tools (Midjourney, Firefly, and
similar). Adapt syntax per tool; the substance stays constant.

This is the **assembly map**, not a standalone prompt. It holds the prompt's structure, the variable
slots, and the tokens native to it (material, style references, the negative list), and it **points
to the canonical homes** — [`color.md`](color.md) for palette, [`treatment.md`](treatment.md) for
optics, lighting, and mood, and [`../governance-rules.md`](../governance-rules.md) for the
compositional rule — for everything that lives elsewhere. The `prompt-architect` skill reads this map
plus those files and the relevant subject file, then assembles the full prompt. Nothing here restates
what those files own, so they can't drift apart.

## Structure

\`\`\`
[SUBJECT]: <variable — what is being shown; add a temporal token if era drifts, see below>

[MATERIAL]: a seamless coexistence of precision-engineered and living/grown materials —
   matte surgical steel, raw board-formed concrete, gold accents, brushed ceramic,
   integrated with living moss, mycelium-grown composites, raw and cultivated timber,
   preserved botanical specimens in resin, bone-white biocomposite, woven plant fiber
   + <subject-specific materials>

[OPTICS] → canonical in treatment.md
   medium-format register, f/5.6–8, hyper-sharp, low saturation, neutral midtones, no HDR;
   focal length by subject (100mm macro / 80mm portrait / 35mm interior / 24mm architecture)

[LIGHTING] → canonical in treatment.md
   single directional 5600K daylight, no fill, no gels; emissive accents amber 2700K
   point-source, no bloom/halo; primary direction and hardness by subject

[COMPOSITION]
   Locked → governance-rules.md Rule #03: specimen-presentation, architecture-dominant,
      generous negative space (~40%), documentary register, no hero angles
   Variable by shot type:
      Object/specimen: centered, isolated, plinth/vitrine implied
      Architectural interior: rule-of-thirds, figure ~10–20% of height, architecture fills remainder
      Editorial/data: Swiss grid logic, type-driven hierarchy

[STYLE REFERENCE]
   Locked (always): Neri Oxman Material Ecology register, Hiroshi Sugimoto tonal precision
   Variable by shot type:
      Object/specimen: + Massimo Vignelli editorial restraint
      Architectural/environmental: + Tadao Ando interior architecture
      Editorial/data: + Vignelli + Swiss International Style grid logic

[PALETTE] → canonical in color.md
   matte-black / concrete-grey / off-white / timber / bone-white grounds; gold = matter,
   amber = light; editorial accents (mustard, fuchsia, chartreuse, cobalt, plum, red),
   each flat and bounded, ≤10% of frame, one accent per composition

[MOOD] → canonical in treatment.md
   clinical precision married with living attention; "the nerves in the numbers"; fails if it
   lands only cold or only warm (the two failure lists live in treatment.md)

[ASPECT]: <variable — 4:5 object/specimen, 16:9 architectural, 3:2 or 1:1 editorial/data>

--no neon, glow, halo, lens flare, chrome reflection, glossy surface, blue gradient, purple
gradient, holographic, padlock, shield, neural network, glowing nodes, futuristic UI, hacker
imagery, hooded figure, command center, multiple monitors, LED strips, exposed wires, sci-fi
tropes, cyberpunk, dystopian, dramatic bokeh, motion blur, HDR, oversaturation, stock office,
white seamless background, Midjourney sheen, sterile lab, clinical white biotech, futuristic
greenhouse, crypto-bro gold, tropical green, lifestyle warmth, heroic figure, low-angle hero shot
   (the conceptual territories behind this list live in ../anti-patterns.md)
\`\`\`

## Known weak seam — temporal register

The scaffold encodes era *implicitly*, through materials and named references. When text alone is
used (no image reference), outputs drift toward present-moment register rather than 2035
speculative. If this drift appears, add an explicit temporal token to the SUBJECT line:

- "speculative architectural photography 2035"
- "documentary of a not-yet-existing institution"
- "post-current ground truth infrastructure"

A v2 of the scaffold should add a standing TEMPORAL token (see [`../../PLAN.md`](../../PLAN.md)
backlog and `decisions/`).

## Notes on style references in image tools

- Image references override text prompts on whatever attributes they carry strongly — including
  unintended secondary qualities (gloss, environment, plinth treatment). Use only references that
  fully embody what you want, including the secondary qualities you did not mean to anchor.
- Strongest anchors identified so far: brutalist concrete with oculus light (material + light
  register), Neri Oxman Material Ecology documentation (precision-organic synthesis), museum
  specimen-vitrine images (composition posture).
- When a reference pulls the output unintentionally, lower style weight aggressively (`--sw 50` or
  below) or remove the reference and rely on text.
