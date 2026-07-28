# CLAUDE.md — how an AI agent operates in this repo

This repository is the canonical source of the Tenet Ground brand. Everything that defines the
brand — what it stands for, how it speaks, how it looks, and the rules governing every generated
asset — lives here as plain markdown, written once, so people and models read from the same truth.

If you are a model picking this up cold, read this file first, then `README.md`, then the reading
order below. You will be current in about ten minutes.

---

## Reading order

1. **`brand/foundation.md`** — the bedrock. Everything answers to it.
2. **`brand/audience.md`** — who this is for, and the three-tier model that explains the business.
3. **`brand/governance-rules.md`** — the four rules, each with a pass/fail test. Every asset is
   checked against these.
4. **`brand/beliefs.md`, `voice.md`, `messaging.md`, `lexicon.md`, `anti-patterns.md`** — the verbal
   system.
5. **`brand/visual/`** — the visual system. `treatment.md` and `color.md` are canonical for optics
   and palette; `marks.md` for geometry; `typography.md` and `logo.md` for type;
   `prompt-scaffold.md` assembles image prompts; `ground-ring.md` and `ground-hall.md` are the two
   canonical rendered subjects.
6. **`brand/surfaces/`** — specs for anywhere the brand is *read* rather than rendered.
7. **`brand/decisions/`** — read last, in date order. **This is the state of the brand.** Every
   position that has been settled, and why, in an append-only log.

---

## The five operating principles

These are load-bearing. They were each learned the hard way and are the most expensive things to
rediscover.

**1. Specify behavior, not presence.** Naming a thing does not constrain how it acts. "Matte black"
rendered glossy until the spec said *PVD-coated, non-reflective, absorbing light rather than
reflecting it.* Rules that ban a *form* break repeatedly; rules that constrain a *behavior* hold.
This has been rediscovered on screens, on floating displays, on transitions, and on iconography.
Apply it globally before writing any new rule. See `decisions/behavior.md`.

**2. The model builds the world; the designer authors the system.** An image model's brand-carrying
competence is material and light — which is why the Ground Ring and the Ground Hall lock well.
Grid, type scale, data density, hierarchy and state are not material properties, and no model holds
them. Prompting for a surface returns a photograph of a surface-shaped object with rendering where
the design decisions should be. **A model may render a plane; it may not compose what is on it.**
See `surfaces/README.md`. The full argument, and its portability beyond this project, is in [`METHOD.md`](METHOD.md).

**3. Fidelity to the manifesto beats aesthetic distinctiveness.** When a productive drift forces a
choice, the brand-functional option wins over the more arresting one. Aesthetic preference
unconnected to brand logic is the most common source of drift. See `decisions/forms.md`.

**4. A rule that blocks an authored decision has outlived its scope — but overriding it requires a
brand-functional reason.** Many rules were written against the model's defaults, not for the brand.
When a considered human decision hits one, the rule can be amended. The standard is: *can you state
the reason in terms of ground truth, verification, recessiveness, or the numbers-have-nerves
thesis?* "It looks good" is drift wearing a nicer outfit.

**5. Productive drift is data, not failure.** When a generation pulls somewhere unexpected, that
usually surfaces an unmade brand decision rather than a rendering error. Record it.

---

## How to propose a change

**Never edit a canonical file quietly.** The audit trail is the point.

1. Confirm the change against `governance-rules.md` and the principles above.
2. Write a decision record in `brand/decisions/`, named `YYYY-MM-DD-short-slug.md`, using the format
   in `decisions/README.md`: what changed, why, what it supersedes.
3. Make the edits the record describes.
4. If the change resolves an open item in another file, close it there too.

A record that only says what changed is half a record. The *why* is what makes the system
defensible a year later.

---

## Conventions

- **One idea per file.** If a file needs to say two things, it is two files.
- **Point, do not restate.** Each fact has one canonical home; other files link to it. This is what
  stops the system drifting apart. If you find yourself copying a value between files, you have
  found a missing pointer.
- **Frontmatter** on every canonical file: `title`, `type`, `status`, `updated`, `source`.
- **Open items** live at the bottom of the file they belong to. State a position and flag it rather
  than leaving a blank — an overruled position is more useful than an absence.
- **Links are relative** and must resolve on GitHub. Check them after any rename.
- **Never invent an unspecified value.** If a colour, size, or spec is not written down, say so and
  add an open item. Guessing is how a palette accumulates instead of being authored.

---

## Checking an asset

Walk it through the four governance rules in order. Each has a pass/fail test:

1. **Technology presence** — if you identify the technology before the architecture, it failed.
2. **Colour behavior** — if any colour is gradient, glowing, washing or bleeding, it failed,
   regardless of hue.
3. **Compositional authority** — if the subject feels heroic rather than presented, it failed.
4. **Typographic neutrality** — if you notice the typeface before you read the value, it failed.

Then check the two register failures in `visual/treatment.md`: an asset can satisfy all four rules
and still fail by landing only cold or only warm.

A failing rule names the scaffold token that needs reinforcing.

---

## What is not in this repo

`README.md` describes a fuller structure than currently exists. These are known gaps, not missing
files to hunt for:

- **`skills/`** — the four named skills (`prompt-architect`, `image-reviewer`, `copy-reviewer`,
  `ring-fidelity-checker`) are designed but not written.
- **`assets/`** — the media library. Renders, UI artwork and design sources live outside the repo
  and are not yet indexed.
- **`examples/`, `PLAN.md`** — not written.
- **`logo.svg` / `logo-reversed.svg`** — the logotype is specified in `visual/logo.md` but the
  vector masters are not committed.

Binaries do not belong in this repo. SVG is text and may live here; raster exports do not.

---

## One thing to understand about this brand

Tenet Ground's product is a canonical specification that people and machines read from, so that
every verification produces the same result anywhere. This repository has the same form as the
business it describes. That is not a coincidence to point out in the work — but it is why the
governance is not decoration on top of the brand. It *is* the brand.

One system. One intent.
