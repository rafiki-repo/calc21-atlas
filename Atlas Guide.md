---
type: meta
status: draft
updated: 2026-11-13
---

# Atlas Guide

How this Atlas is organized, and how far to trust it. Written for human readers first and for the agent that maintains it second.

## What this is

A **map** of calculus. Each note is short: what the thing is, why it's interesting, and where to go next. We link to good explanations rather than rewriting them.

## How to read it

1. Begin at [[Home]], or follow a trail in [[Rabbit Holes]].
2. Every note ends with a **Next stop** section to keep you moving.
3. Use [[Glossary]] when a term is unfamiliar.
4. Check [[What's New]] to see what changed recently.

## Note labels

Each note has a `status` in its header:

- **stub** — a placeholder with little content
- **draft** — useful but not fully checked
- **solid** — reviewed and cross-linked

Notes about open problems, recent claims, or living people also carry a `last_checked` date. Claims there are attributed, and preprints or announcements are labeled as such. Anything marked `unverified-seed` was written from general knowledge and still needs a source check.

## Layout

| Folder / file | Purpose |
|---|---|
| `Home.md` | Front door |
| `Rabbit Holes.md` | Guided trails across sections |
| `What's New.md` | Human-readable recent changes (newest first) |
| `Atlas Guide.md` | This page |
| `Concepts/` · `People/` · `Stories/` · `Open Problems/` · `Puzzles/` · `Applications/` · `Education/` · `Resources/` · `Frontiers/` | Content sections. Each folder has a hub note with the same name as the folder. |
| `Glossary/Glossary.md` | One note, alphabetical headings; link to a term with `[[Glossary#Term]]` |
| `Meta/Templates/` | Note templates for each note type |

## Conventions (for the maintaining agent)

- **Filenames are titles** in plain Title Case, no special characters (so links stay simple and the site sync is safe).
- **Link generously** with wikilinks (double square brackets). No orphans: every note is listed in its section hub and ideally linked from at least one other note.
- **Frontmatter** on every note: `type`, `status`, `updated` (YYYY-MM-DD). Add `last_checked`, `tags`, and `sources` where relevant.
- **Every content note** has a one-line hook at the top, a short body, and a **Next stop** section with 2-4 links to related notes.
- **Keep it lean.** Notes are a screenful or two. Prefer improving an existing note to adding a near-duplicate.
- **Wording follows the editorial guardrails:** attribute claims, label preprints, no hype, no prescriptions. Only link to pages that were actually fetched and checked.
- **After each run:** update the relevant section hubs, add an entry at the top of [[What's New]], and consider adding the new material to a trail in [[Rabbit Holes]].
- Don't hard-code the dates of "what's recent" in hub notes; that belongs in [[What's New]].
