---
title: Restructure the research repo and bring the research-group material home
type: plan
status: done
updated: 2026-10-26
---

# Restructure the research repo

## Purpose

Make `life-itself/research` the one home for the research group's material, in the classic Life Itself repo shape, and published as a whole. At the moment the group's history, charter, sources and purpose LTP sit in the private `life-itself/sor-community` repo, and this repo holds only the old site.

Decided by Rufus, 26 Oct 2026. Background: the web LTP in sor-community (`projects/2026-10-research-community/ltp/context.md`, conflict clouds accepted 26 Oct) picked this repo as the research group's reference repo. It stays public.

## Outline

1. Keep everything at the root. Hide what shouldn't publish with Flowershow's `contentExclude`. No `site/` subfolder.
2. Spread the sor-community research-group material across this repo by kind: core documents at the root, reference material in `ref/`.
3. Bring both LTPs across. The purpose LTP (LTP 1) is core to the group, so it goes at the root. The web LTP (LTP 2) belongs to a bounded project, so it goes in `projects/`.
4. Leave stubs in sor-community.
5. Each LTP moves when it is complete, and the session that ran it does the move. The purpose LTP is published only after its wording pass.

## Target layout

```
README.md          site home page (as now)
history.md         the group's history          (from sor-community)
vision.md          vision and inspirations      (from sor-community)
pattern.md         governance charter, Apr 2026 (from sor-community)
purpose-ltp/       LTP 1: the group's purpose and relaunch (from sor-community)
discovery-calls.md as now
ref/               reference material: sources inventory, sub-circle charter template
projects/          bounded work: the 2022-25 project pages (as now) and new project folders,
                   e.g. projects/2026-10-research-community/ (LTP 2, from sor-community)
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
| `sources.md` | `ref/sources.md` (26 Oct, after trimming personal remarks and a contact address; Google Doc links kept) | reference |
| `sub-circle-charter.md` | `ref/sub-circle-charter.md` | template that goes with the pattern |
| `archive/inspirations-board-2023.jpg` | `assets/inspirations-board-2023.jpg` | used by `vision.md` |
| `archive/where-next-for-2025.md` | none | already published here as `posts/where-next-for-2025.md`. Keep the post and drop the copy, after checking they match |
| `archive/README.md` | none | its index is no longer needed |
| `purpose-ltp/` (context, goal options, YAML, `.gitignore`) | `purpose-ltp/` | LTP 1, core to the group. Do not move `.reason-commons/`, which is generated and gitignored. Moved by the research-ltp session after the wording pass |
| `README.md` | stays in sor-community as a stub | points to this repo |

From sor-community `projects/2026-10-research-community/`:

| From | To | Note |
|---|---|---|
| `README.md` (SCQ B) and `ltp/` (context, YAML, `.gitignore`) | `projects/2026-10-research-community/` | LTP 2, the web and knowledge presence project. Same rules on `.reason-commons/`. Moved by the research-web-ltp session when its LTP is done |
| — | sor-community keeps a one-line row in `projects/README.md` pointing here | |

## Steps

1. **Now:** add this plan, exclude `/docs/plans` from the site, and delete the stray `.beads.gate.lock`.
2. **When the research LTPs are complete:**
   1. Check the files for anything that shouldn't be public. sor-community is private because it holds notes on members.
   2. Rewrite links:
      - Links to sibling repos (`../../../next.lifeitself.org/...`, `../../../planning/...`) become GitHub URLs.
      - Links back into sor-community become GitHub URLs, noting that the repo is private.
      - Internal links get their new paths.
   3. Move the core and reference files as in the table (this thread).
   4. Each LTP session moves its own LTP, copying the files across, then removing them from sor-community, with the same link rules. Each also fixes the cross-links between the two LTPs, since the web LTP reuses purpose LTP nodes.
   5. Link the new pages from the home page if they belong there (history, vision, pattern, purpose LTP).
3. **In sor-community:**
   1. Turn `initiatives/research-group/README.md` into a stub that points here.
   2. Replace `projects/2026-10-research-community/` with a row in `projects/README.md` that points here.
   3. Update the links in `initiatives/README.md` and anything else that points at the moved files.
   4. Check `planning/initiatives/life-itself-research.md`.
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
