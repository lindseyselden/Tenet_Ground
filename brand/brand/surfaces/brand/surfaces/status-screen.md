# brand/surfaces/ — the surface specs

A **surface** is anywhere the brand is read: a status screen, a web hero, signage, a deck, a document,
a card. This folder holds one spec per surface.

Surfaces are specified separately from subjects for a reason. `visual/ground-ring.md` and
`visual/ground-hall.md` specify **things** — their brand-carrying properties are material, light, and
form. A surface's brand-carrying properties are **grid, type scale, density, hierarchy, and state**.
Those are authored, not generated, and they need their own kind of file.

[`../voice.md`](../voice.md) points here for register and length: the voice is constant, the register
shifts with the surface, and the surface file is the single source for that shift.

## The skeleton

Every surface file carries these sections, in this order:

| Section | What it holds |
| --- | --- |
| What it is | Where the surface appears, who reads it, what question it answers |
| Register | Length and tone for this surface, narrowed from `voice.md` |
| Grid & structure | Columns, rows, margins, division logic |
| Type | Which of the three faces, in which role, at which scale |
| Data density | How much information, ranked how |
| Color application | Which tokens, what they mean here, what percentage |
| States | Every state the surface can be in, and how it changes between them |
| Governance | How Rules #01–#04 land specifically on this surface |
| Forbidden | Surface-specific failure modes |
| **Generated vs. authored** | Which layers come from a model, which are drawn, and the workflow rule |
| Open items | Unresolved design calls, stated rather than left blank |

Not every surface needs every section — a printed document has no states — but the order stays fixed
so the files are comparable.

## Generated vs. authored

This section is required and is the point of the folder. Each surface declares which layers a model
may produce and which are authored, with a one-line workflow rule stating how the two are combined.
Where a spec is silent, the default is: **the model builds the world; the designer authors the
system.**

## Status

| Surface | File | Status |
| --- | --- | --- |
| Status screen | [`status-screen.md`](status-screen.md) | draft |

Planned: web hero, signage, editorial/document, deck.
