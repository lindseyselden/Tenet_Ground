---
title: Governance Rules
type: governance
status: active
updated: 2026-06-18
source: original governance document (three operational rules + two principles)
---

# Governance Rules

The governance rules sit **above** the prompt scaffold. The scaffold is tactical ("what to type");
the rules are strategic ("why we typed that"). Each rule carries a built-in pass/fail test so any
output can be judged against the system. The `image-reviewer` skill runs these tests; the
`prompt-architect` skill writes prompts that satisfy them in advance.

## Rule #01 — Technology Presence

**Always specify:** integrated, embedded, recessive, flush-mounted, single surface.
**Always avoid:** screens, displays, multiple monitors, bezels, LED strips, command center,
futuristic UI, electronics, cables.

**Pass/fail test:** If you can identify the technology before you identify the architecture, the
shot has failed.

**Why:** Tenet Ground is ground truth infrastructure. Infrastructure is recessive by definition. A
brand that *performs* its technology contradicts its promise of quiet authority. Most security and
SaaS brands fail this rule by default; Tenet Ground's position depends on holding it.

## Rule #02 — Color Behavior

**Always specify:** flat, bounded, editorial, low saturation, neutral midtones.
**Always avoid:** gradient, glow, atmospheric, halo, bleeding, washing.

**Pass/fail test:** Does any color in the frame behave atmospherically — gradient, glowing, washing,
bleeding into shadows? If yes, the shot has failed regardless of hue.

**Why:** The hue is not the rule; the *behavior* is. Tenet Ground can use any color — including the
blues and purples the anti-territories warn against — as long as it appears editorially: flat,
bounded, spotted, intentional. What is forbidden is color behaving as atmosphere or "tech
signifier." This rule lets the brand use a richer accent palette than it might appear to allow. See
[`visual/color.md`](visual/color.md).

## Rule #03 — Compositional Authority

**Always specify:** specimen presentation, architecture-dominant, generous negative space,
documentary framing.
**Always avoid:** hero shot, dramatic angle, dutch tilt, low-angle, candid, heroic.

**Pass/fail test:** If the subject feels heroic — centered and aggrandized rather than presented —
the shot has failed. Architecture should dominate the figure; the human operates precisely within
infrastructure, not heroically against it.

**Why:** The brand thesis is the *system* over the individual. "One system. One intent." The
compositional logic must make this visually true. Generic security imagery makes the executive a
hero in a command center; Tenet Ground does the opposite — the infrastructure is the hero, the
Integrity Architect is the precision within it.

## Rule #04 — Typographic Neutrality

**Always specify:** neutral system typefaces, recessive, value read before the face, idiosyncrasy
reserved for the logotype.
**Always avoid:** expressive or display faces, decorative letterforms, type as the message, branded
type outside the logotype.

**Pass/fail test:** If you notice the typeface before you read the value, the type has failed.

**Why:** Infrastructure is recessive — including its type. The system speaks; the typeface doesn't
perform. The one place idiosyncrasy is permitted is the logotype. The type system itself lives in
[`visual/typography.md`](visual/typography.md).
---

## Two principles that animate the rules

Two principles sit beneath the three rules — load-bearing, but not standalone tests, so they live
canonically elsewhere and are only referenced here:

- **The Numbers Have Nerves** — the emotional thesis (clinical precision married with living
  attention; the cold/warm failure) the three rules exist to protect. Stated in
  [`beliefs.md`](beliefs.md).
- **The System Is Uniform; The Signature Is Individual** — the Ground Ring's locked-exterior,
  variable-interior logic, extensible to other personal tools. Stated in
  [`visual/ground-ring.md`](visual/ground-ring.md).

---

## How to use these rules

- **Before generating:** confirm the prompt reflects each "always specify" directive and includes
  the "always avoid" terms in the negative list. `prompt-architect` does this by construction.
- **After generating:** walk the output through all three pass/fail tests in order. If it fails, the
  failing rule names the scaffold token that needs reinforcement. `image-reviewer` does this.
- **When designing a new asset type** (portrait, UI, motion, print): the three rules generate the
  constraints for asset types the scaffold has no specific recipe for yet.
- **When in conflict with aesthetic preference:** the rules win. Aesthetic preference unconnected to
  brand logic is the most common source of drift. (See `decisions/` for the case that established
  this.)
