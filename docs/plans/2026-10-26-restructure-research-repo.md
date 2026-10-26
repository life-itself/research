---
title: Restructure the research repo and bring the research-group material home
type: plan
status: active
updated: 2026-10-26
---

# Restructure the research repo

## Purpose

Make `life-itself/research` the one home for the research group's material, in the classic Life Itself repo shape, and published as a whole. At the moment the group's history, charter, sources and purpose LTP sit in the private `life-itself/sor-community` repo, and this repo holds only the old site.

Decided by Rufus, 26 Oct 2026. Background: the web LTP in sor-community (`projects/2026-10-research-community/ltp/context.md`, conflict clouds accepted 26 Oct) picked this repo as the research group's reference repo. It stays public.

## Outline

1. Keep everything at the root. Hide what shouldn't publish with Flowershow's `contentExclude`. No `site/` subfolder.
2. Spread the sor-community research-group material across this repo by kind: core documents at the root, reference material in `ref/`, the purpose LTP in a project.
3. Leave a stub for the research group initiative in sor-community.
4. Do the move only once the research LTPs are complete, and publish the purpose LTP only after its wording pass.

## Target layout

```
README.md          site home page (as now)
history.md         the group's history          (from sor-community)
vision.md          vision and inspirations      (from sor-community)
pattern.md         governance charter, Apr 2026 (from sor-community)
discovery-calls.md as now
ref/               reference material: sources inventory, sub-circle charter template
projects/          bounded work: the 2022-25 project pages (as now) and new project folders
publications/      as now
posts/             as now
archive/           older material kept for reference
assets/            images and PDFs
docs/              how to use this repo (published)
docs/plans/        near-term plans like this one (not published)
raw/, templates/   not published (as now)
initiatives/       only when there is an ongoing initiative to record
```

Why no `site/` folder: Rufus wants to publish most of this, including the LTP. A root layout does that with no special handling, keeps existing URLs working, and needs no change in the Flowershow dashboard. Flowershow does support a root directory setting, so we can add a `site/` folder later if we need one.

Why no `initiatives/research-group/`: the research group initiative is this whole repo. Its material spreads across the repo rather than sitting in one folder.

## Where the research-group material goes

From sor-community `initiatives/research-group/`:

| From | To | Note |
|---|---|---|
| `history.md` | `history.md` | core |
| `vision.md` | `vision.md` | core |
| `pattern.md` | `pattern.md` | core: the governance charter |
| `sources.md` | `ref/sources.md` | reference |
| `sub-circle-charter.md` | `ref/sub-circle-charter.md` | template that goes with the pattern |
| `archive/inspirations-board-2023.jpg` | `assets/inspirations-board-2023.jpg` | used by `vision.md` |
| `archive/where-next-for-2025.md` | none | already published here as `posts/where-next-for-2025.md`. Keep the post and drop the copy, after checking they match |
| `archive/README.md` | none | its index is no longer needed |
| `purpose-ltp/` (context, goal options, YAML, `.gitignore`) | `projects/2026-10-research-relaunch/ltp/` | the project for the relaunch and this restructure. Do not move `.reason-commons/`, which is generated and gitignored |
| `README.md` | stays in sor-community as a stub | points to this repo |

New: `projects/2026-10-research-relaunch/README.md`, a short project brief covering the purpose LTP, the January 2027 relaunch and this restructure, linked to the Beads epic `sorr-l57`.

The SCQ B project (`projects/2026-10-research-community/`, including the web LTP) stays in sor-community. It is about research's place in SoR.

## Steps

1. **Now:** add this plan, exclude `/docs/plans` from the site, and delete the stray `.beads.gate.lock`.
2. **When the research LTPs are complete:**
   1. Check the files for anything that shouldn't be public. sor-community is private because it holds notes on members.
   2. Rewrite links:
      - Links to sibling repos (`../../../next.lifeitself.org/...`, `../../../planning/...`) become GitHub URLs.
      - Links back into sor-community become GitHub URLs, noting that the repo is private.
      - Internal links get their new paths.
   3. Move the files as in the table, and write the project README.
   4. Link the new pages from the home page if they belong there (history, vision, pattern).
3. **In sor-community:**
   1. Turn `initiatives/research-group/README.md` into a stub that points here.
   2. Update the links in `projects/README.md`, `initiatives/README.md`, the SCQ B README, `ltp/context.md` and `ltp/reason-commons.yaml`.
   3. Check `planning/initiatives/life-itself-research.md`.
4. **Gate:** commit the purpose LTP here only after the wording pass, `sorr-l57.21`. This repo publishes on push.
5. **Beads:** close `sorr-3kr.5`, and note the new paths in `sorr-l57.15`.
6. **Check:** the live site, the home page, `/discovery-calls` and the nav links.

## Risks

- **Private material goes public.** The move publishes on push, so step 2.1 and the gate in step 4 matter.
- **Links break** across the two repos. Step 2.2 handles them; check the live site afterwards.
- **A short outage** is acceptable. Few people visit the site (Rufus, 26 Oct).
- **Redirects** from research.lifeitself.org to lifeitself.org/research are separate, under `sorr-l57.15`.

## Tasks

Tracked in Beads in this repo (epic: restructure the research repo), not here.
