---
title: The screen plane is a substrate, not a source — free-standing permitted, atmospheric color still forbidden
type: decision
date: 2026-07-28
status: active
changes:
  - brand/governance-rules.md
  - brand/visual/color.md
supersedes: null
---

## What changed

Two things, deliberately separated, because a single render failed for two unrelated reasons.

**Rule #01 (Technology Presence) is amended.** A free-standing screen plane is now permitted, under
conditions. The "always avoid" list drops the blanket ban on *floating or free-standing displays* and
replaces it with the forms that actually perform: framed or bezelled displays, opaque panels that
occlude the architecture behind them, arrays of multiple displays, device chrome, visible mounting
hardware. A single frameless transparent plane, carrying flat data, through which the architecture
remains legible, passes.

The permitting conditions are explicit:

- **Transparent substrate.** The architecture behind the plane must read through it. An opaque panel
  is a display; a transparent one is a surface.
- **Frameless.** No bezel, no housing, no visible mount. The plane appears held rather than installed.
- **One plane per sightline.** Comparison is a division within the plane — a grid, not a second
  screen. Repeated adjacent planes read as an array, and an array is a command center.
- **The plane emits nothing.** Data sits *on* the surface, flat and bounded. The substrate is not a
  light source.

The pass/fail test is unchanged: *if you can identify the technology before you identify the
architecture, the shot has failed.* A transparent plane passes it on its own terms — which is why the
literal ban was the wrong instrument.

**Rule #02 (Color Behavior) is unchanged, and reaffirmed.** The chartreuse in the UI WIP was not the
failure; `color.md` already sanctions chartreuse for live data and verified signals. The failure was
*behavior* — the mint rendered layered, semi-transparent and bleeding across the plane, which Rule #02
forbids regardless of hue or substrate.

A distinction is added to `color.md` to stop this recurring:

> **Substrate transparency is not color transparency.** The plane may be transparent. The data on it
> may not. Marks render flat, bounded and fully opaque against a transparent ground — the same way
> ink sits on glass, not the way light passes through it.

## Why

Both rules were written early, against the model's defaults, at a point when every generation was
drifting toward command-center and tech-glow. They did their job. But Rule #01 had over-indexed on the
token *floating* in the same way it once over-indexed on *screens* — naming a form rather than the
behavior the form usually carries. The June 19 amendment (`techbehavior.md`) already established that
this rule governs how technology behaves; this extends the same correction one step further.

The trigger was a specific render: a transparent plane set against board-formed concrete beside a
dark door. It reads architecture first — concrete, threshold, raking light — and the plane second,
because the wall is visible through it. It passes Rule #01's actual test while failing its literal
avoid-list. That gap is the rule's problem, not the render's.

The render *did* fail Rule #02, for reasons that have nothing to do with floating. Collapsing the two
failures into one verdict would have retired a good rule to fix a bad one.

There is a second reason to make this change deliberately rather than by exception. The rules exist to
suppress the model's defaults, not the designer's judgement. When a considered, authored decision is
blocked by a rule written to catch a machine cliché, the rule has outlived its scope. The standard for
overriding remains the one set in `forms.md` — a brand-functional reason, not an aesthetic preference.
Here the reason is that a transparent plane is *more* recessive than a flush opaque one: it occludes
nothing.

## What this supersedes

Amends Rule #01's avoid-list, extending — not reversing — `techbehavior.md` (2026-06-19). The
recessiveness rationale and the pass/fail test stand unchanged.

Rule #02 is not amended. The clarification added to `color.md` names a distinction the rule always
implied.

Asset-level specs are unaffected. The Ground Ring keeps "no screen" and the Ground Hall keeps "no
command-center monitors" — both remain correct for those subjects. The Ground Hall's flush-mounted
signage and elevator type system are unchanged and remain the canonical recessive screen.
