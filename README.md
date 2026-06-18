# Tenet Ground — Brand System

**Tenet Ground** establishes the Ground Truth Infrastructure for autonomous commerce — the
foundational layer that verifies behavioral intent in a world where seeing is no longer believing.

This repository is the **canonical source of the brand**. Everything that defines Tenet Ground —
what it stands for, how it speaks, how it looks, and the rules that govern every generated asset —
lives here, in one organized place, written once. It is built so **both people and AI tools** read
from the same truth. **You do not need to know how to code.**

---

## New here? Read this first

A few terms, plainly:

- **This page (a "repository" or "repo")** — a tidy collection of text files shown on GitHub. Click
  any folder or file to open it. Nothing here runs or breaks.
- **`.md` files** — plain-text files (*Markdown*) that display as formatted pages in your browser.
- **A "skill"** — a page of instructions you paste into an AI chatbot (like [claude.ai](https://claude.ai))
  so it generates or reviews work **in the Tenet Ground voice and look**. A recipe: paste it in,
  attach the brand files it names, get an on-brand result.
- **The media library** — images and renders live in one external folder (link in [`assets/`](assets/README.md)),
  not in this repo, so this stays light.

---

## What do you want to do?

| I want to… | Go here |
| --- | --- |
| **Understand the brand** (manifesto, voice, look) | Open [`brand/`](brand/README.md) and start with `foundation.md`. |
| **Generate an on-brand image prompt** | Use the **prompt-architect** skill — see [How to use a skill](#how-to-use-a-skill-step-by-step). |
| **Write something on-brand** (manifesto, web hero, signage) | Use the **brand-writer** skill. |
| **Check a generated image against the brand** | Use the **image-reviewer** skill (it runs the three governance rules as pass/fail). |
| **Check a Ground Ring render is on-spec** | Use the **ring-fidelity-checker** skill. |
| **Get the renders and reference images** | Open the [media library](assets/README.md). |

---

## How to use a skill (step by step)

No coding. If you can copy, paste, and attach a file, you can do this.

1. **Open the skill.** Go to [`skills/`](skills/README.md), open the category folder (**generation**,
   **strategy**, **governance**, or **brand-transform**), then the skill, and open its `SKILL.md`.
   Select all the text and copy it.
2. **Open an AI chatbot** and paste it in.
3. **Attach the brand files it asks for.** Near the top, each skill names the files it needs (e.g.
   `governance-rules.md`, `visual/prompt-scaffold.md`). Download those from [`brand/`](brand/README.md)
   and attach them.
4. **Tell it what you need** — e.g. *"A macro prompt for the Ground Ring on a concrete plinth."*
5. **Done.** It replies on-brand. Iterate like a normal conversation.

> Why attach files? Skills never copy the brand rules into themselves — they point to the real brand
> files so there is only ever **one source of truth**. You bring those files along.

---

## The toolbox (skills)

**Generate**

- **prompt-architect** — builds an image-generation prompt from the master scaffold + governance
  rules for a named subject (the Ground Ring, the Ground Hall, an editorial frame).
- **brand-writer** — on-brand copy for a named surface (manifesto, web hero, signage, press, social).
- **name-forge** — names in the `Ground [X]` system (and judges when the pattern stops serving).
- **voice-rewriter** — rewrites any text into the Tenet Ground voice.

**Strategy**

- **narrative-strategist** — positioning and campaign concepts for an objective.

**Govern** (check before it ships)

- **image-reviewer** — scores a generated image against the three governance rules. Pass/fail.
- **copy-reviewer** — scores copy against voice and the anti-territories.
- **ring-fidelity-checker** — checks a Ground Ring render against the canonical product spec.

**Evolve**

- **brand-evolver** — proposes and writes updates to the brand, logging each change to `decisions/`.

---

## What's in here

| Folder | What it holds |
| --- | --- |
| [`brand/`](brand/README.md) | **The brand itself**, one idea per file: foundation, beliefs, voice, lexicon, the governance rules, the surfaces, and the visual system (including the master prompt scaffold and the two canonical subjects). Start here. |
| [`assets/`](assets/README.md) | A pointer to the external media library and a machine-readable index of approved renders. No binaries live here. |
| [`skills/`](skills/README.md) | The AI tools above. |
| [`examples/`](examples/README.md) | Worked end-to-end chains showing the skills used together. |
| [`PLAN.md`](PLAN.md) | The durable build plan and progress checklist. |
| [`CLAUDE.md`](CLAUDE.md) | How an AI agent operates in this repo. Safe to ignore for everyday use. |

---

## The one idea behind all of this

The brand is written down **once**, in plain files, so every person and every tool works from the
same truth. Generate something, govern it against the rules, ship it. No scattered docs, no
guesswork, no "which version is right."

One system. One intent.
