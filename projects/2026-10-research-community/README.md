# Research community — web and knowledge presence (SCQ B)

Status: SCQ B signed off 2026-10-23 by Rufus (criteria marked (guess) accepted as working values)
Source: conversation with Rufus, 22–23 Oct 2026. Beads epic: `sorr-l57` (this repo; formerly `calls-kwd` in sor-community).

How research's web and knowledge presence fits into Seeds of Renaissance (SoR). The research group's purpose (SCQ A) was answered in a separate LTP: see the [purpose LTP](../../purpose-ltp/README.md). This project takes its outputs as inputs and does not reopen them. Shared background: [history.md](../../history.md) and [sources](../../ref/sources.md).

## SCQ B — web and knowledge presence

### Situation

- **New SoR website.** seedsofrenaissance.org is being built in the private `life-itself/sor-website` repo (Astro on Cloudflare Pages, still marked draft; the ~23 Oct target slipped; 1 Nov launch). It replaces secondrenaissance.net, whose pages are migrated with redirects; lifeitself.org stays as is (planning `2609`, sor-website `docs/project.md`, read 23 Oct).
  - Its site brief (22 Oct) says the research collective gets "its own subsite", with a need-led entry on the Join page ("want better research on these subjects? Here is a group doing it") and a footer link. Nothing about research is built yet.
- **research.lifeitself.org.** A Flowershow site from the public `life-itself/research` repo, still live. Last content change Nov 2025. Holds 2022–25 projects, ten publications, two posts and the discovery-calls page; its navbar points to the Substack and the old 2R forum.
- **lifeitself.org/research.** The research section of the Life Itself site (`next.lifeitself.org` repo). In May 2026 the subdomain's content was copied there as phase 1 of a plan that decided to retire research.lifeitself.org with redirects. The retirement was not done, so the same material is in two places.
- **Other channels.** Substack (lifeitselfresearch), the forum (moving to Forum Magnum), YouTube, Discord, Luma for the Friday calls.
- **Reference material.** The charter, history, sources and purpose LTP sat in the private sor-community repo until 26 Oct 2026. Plan (Rufus, 23 Oct): when this SCQ and the LTP are done, move them to `life-itself/research`, which stays public.
- **The group.** It is now the SoR research group in practice. The SoR funnel is discover → calls → deeper → catalyst, and research is not part of it yet. The purpose LTP decided (Rufus, 22 Oct) on a front of house / back of house split: one moderated public channel for published work (Substack or a renewed forum, not yet chosen), the forum as a back room, and a website for home, history and how to get involved.

### Complication

- Research has no place in SoR. Nothing in the SoR funnel or site leads to it, so SoR members drawn to research have no way in, and the LTP's contributor ladder has no on-ramp.
- The web presence is split and partly stale. No single place presents the work and its history well, and the 2026 migration stopped halfway, so there are two overlapping research homes.
- It is unclear what each site and repo is for: reference knowledge base, public site, or published-work channel. The SoR site brief has pencilled in "its own subsite" without saying what that subsite does. Until that is settled, the LTP's website step (W1), the repo move and any relaunch can't be planned.
- Beyond the websites, it is unclear how the research effort fits into SoR's wider community development and strategy. This may belong to a broader SoR strategy question; flagged here, not resolved.

### Question

What set of research websites and repos, each with a clear job, gives the research group a home in SoR that presents its work and history and connects people to it?

Criteria:
- By when: answered by Fri 30 Oct 2026 (guess, from "nowish").
- For whom: SoR community members, and the SoR / Life Itself community team that runs community development (Gardens of Change in planning) (Rufus, 23 Oct). Also prospective contributors, the research group itself (stewards, members, agents) needing a reference base, and outside readers (guess).
- Effort: Rufus plus agent time; no paid development (guess).
- Off the table: reopening the purpose LTP's decisions (goal, front/back of house); new platforms beyond the existing ones (the Astro SoR site, Flowershow, the current channels) (guess).

Issue tree:
- What research websites and repos are there, and what is each for? — open
  - Do we have a research reference repo or knowledge base? — proposed: yes, `life-itself/research` (Rufus, 23 Oct)
  - Does any of that reference material get published? If so, where, and how does it differ from the Substack and the public site? — open
  - Does the research repo's site move into a subfolder, with the rest of the repo as the knowledge base? — open
- Where does the public research home live: a section of the SoR site, a subsite, or lifeitself.org? (= LTP W1) — open; the SoR site brief proposes a subsite (22 Oct)
  - Does the SoR site need an overall structure plan first (sections, subsites)? — open
- What happens to the old Life Itself research material and to research.lifeitself.org: keep as is, archive, merge or retire? — open
- How do people get from the SoR funnel and the SoR website (Join page, footer) into the research ladder? (= LTP F1) — open
- How does the research effort fit into SoR's wider community development and strategy? — open; may belong to a broader SoR strategy question (planning `initiatives/seeds-of-renaissance/strategy.md`)
- Inputs from SCQ A, not branches here: which channel is the front of house (LTP D1); the group's name and identity.

## Ideas offered (parked)

- Move the research repo's site into a subfolder (e.g. `site/`) that Flowershow publishes, and use the rest as the team's knowledge base (Rufus, 23 Oct).
- Retire research.lifeitself.org with 301 redirects to lifeitself.org/research (May 2026 migration brief, `next.lifeitself.org/docs/plans/2026-05-29-research-migration-brief.md`).
- Merge the website with the Substack (LTP W1 wording).
- Research as "its own subsite", with a need-led entry on the SoR Join page and a footer link (SoR site brief, 22 Oct).

## LTP summary

A Logical Thinking Process (LTP) on SCQ B ran 23–26 Oct 2026. Rufus accepted each tree "for now": a working position to build on, not proof. The full state is in [ltp/reason-commons.yaml](ltp/reason-commons.yaml). Several nodes are reused from the [purpose LTP](../../purpose-ltp/README.md) (W1, F1, D3, A1).

How to read it: the **goal tree** says what must be true (critical success factors, CSFs, and necessary conditions, NCs). The **current reality** says what's wrong and why. The **conflict clouds** are the dilemmas and how we broke them. The **future reality** lists the changes (injections) and what they should produce.

### TL;DR

- **Goal:** research has a home in SoR. Newcomers find a clear way in, the people running the group have a working base, and the group has its own public face that is visibly part of SoR.
- **Likely core drivers:** research moved into SoR in practice but not formally (name, brand and home undecided), and it is unclear which channel does what.
- **What we'll do:** a short research page on the SoR site for the way in; Substack as research's one public site; this repo as the working base and reference; the old research sites redirected or kept as a marked archive.

### Goal tree

Status of each necessary condition (NC), as of 26 Oct: ✓ met, ~ partly met, ✗ not met.

```
G  Research has a home in SoR: a clear way in, a working
   base, and its own public face

CSF1 Way in (core): SoR visitors quickly see what research
     offers, what's next and how to join
 ✓ Home location set: SoR section or subsite (= W1)
   (decided 26 Oct: SoR page + Substack)
 ~ SoR Join page and footer lead to research with
   need-led copy (they point to the old LI page)
 ✗ Research's offer and next call visible and current
 ✗ Paths lead from the SoR funnel to a joinable first
   rung (= F1; the Friday call exists but isn't named)

CSF2 Working base (core): stewards and active members
     find, organise, coordinate and plan in one place
 ~ One public working repo holds docs, plans, tasks
   (this repo, from 26 Oct)
 ✗ Stewards who don't use git can read and update it
 ~ Private material stays out of the public repo
   (checked on the move; privacy rule still to write)

CSF3 Reference (secondary): background docs, past work
     and history are findable
 ✗ Back catalogue has one canonical home (= A1)
 ✗ Reference material findable from the research home

CSF4 Own public face: reaches a wider audience; semi-
     autonomous but visibly part of SoR
 ✓ Front-of-house channel chosen (= D1)
   (decided 26 Oct: Substack)
 ✗ Public face and SoR site link; face is visibly SoR

CSF5 Clear jobs: one job per place, no duplicate homes,
     kept current cheaply
 ✗ Channel map: one job and an owner per place (= D3)
 ✗ New outputs and events reach the home by feed or SOP
 ~ Every site editable as markdown by Rufus and agents;
   no paid development (Substack is the exception)
```

### Current reality

Undesirable effects:

1. The SoR Join page and footer send visitors to a half-migrated Life Itself research page.
2. The first rung of the research ladder isn't stated where SoR visitors land.
3. The next research call isn't shown on a research home; only parts of it appear elsewhere.
4. Working material is split across a private repo, Discord and this repo.
5. The planned public working base sat in a private repo, so its move waited. (Resolved on 26 Oct.)
6. The same back catalogue sits at research.lifeitself.org and lifeitself.org/research; the May 2026 retirement was never finished.
7. research.lifeitself.org is stale, and its navbar points to old channels.
8. New outputs and events never reach the research pages; nothing feeds them.
9. The public face reads as "Life Itself Research", so it isn't visibly part of SoR.

```
C1 Research moved into SoR in practice,   ──► 1  2  6  9
   not formally (name, brand, home)   (likely core driver)
C2 Channel focus unclear; front of house  ──► 3  7  8
   and channel map undecided          (likely core driver)
C3 Thin steward capacity; web work falls  ──► 6  7  8
   to one person (guess)
C4 No simple publishing SOP or feed       ──► 3  8
C5 Tools grew up per channel and project  ──► 3  4  5
C6 The SoR site build pointed research at ──► 1  9
   the existing Life Itself page (guess)
```

C1 and C2 together reach 7 of the 9 effects.

### Conflict clouds

**1. Where research lives**

```
     ┌─ B: Visibly SoR, easy to ── D: A section of the
A:   │    find, cheap upkeep          SoR site
Home ┤                                    ▲ conflict
in   │                                    ▼
SoR  └─ C: Own public face, ────── D′: Its own subsite
          semi-autonomous
```

- **Broken assumption:** "the two can't both exist; one must be the home".
- **Injection:** split the jobs. A short research page on the SoR site is the way in; the public face lives elsewhere (cloud 2).

**2. One public site or two**

```
     ┌─ B: Reference material ──── D: Repo publishes its own
A:   │    findable, presentable       site; Substack for posts
Pub- ┤                                    ▲ conflict
lic  │                                    ▼
face └─ C: One public place, ───── D′: Repo in background;
          cheap upkeep                 Substack is THE site
```

- **Broken assumption:** "reference material needs a proper website to be usable". Reference readers are mainly active members (the CSF3 audience), and the repo serves them.
- **Injection:** Substack is research's one public site; this repo holds reference material, tree state, issues and history, and may keep a low-key site.

**3. Public or private working base**

```
     ┌─ B: The group works in ──── D: Everything in the
A:   │    the open                    public research repo
Work ┤                                    ▲ conflict
-ing │                                    ▼
base └─ C: Privacy and candour ─── D′: The working base
          protected                    stays private
```

- **Broken assumption:** "the working base must be one place".
- **Injection:** split by kind of material. This public repo holds the work. Notes on people stay private. Default public; make private if needed.

### Future reality

| Injection | Mainly addresses effects | Status |
|---|---|---|
| Short /research page on the SoR site; Join and footer point to it | 1, 3 | Decided 26 Oct (cloud 1) |
| Substack is research's one public site, renamed to SoR research | 8, 9 | Decided 26 Oct (cloud 2) |
| This repo is the working base and reference; notes on people stay private | 4, 5 | Decided 26 Oct (cloud 3) |
| research.lifeitself.org redirects; lifeitself.org/research becomes a marked archive | 6, 7 | Decided 26 Oct (cloud 2) |
| Channel map: one job and a named owner per place | 7, 8 | Accepted for now |
| /research page pulls the next call from Luma and posts from Substack | 3, 8 | Accepted for now |
| The SoR team formally accepts research as an SoR group | 1, 9 | Accepted for now; needs the SoR team |
| Friday research call is the first rung until the purpose LTP says otherwise | 2 | To test |
| Decisions and tasks go into Beads, via an agent for stewards who don't use git | 4 | To test |

Main risks, each with a trim in the YAML: the research Substack competing with the SoR newsletter; the custom domain cost; Substack not being editable as markdown; confusion from the rename; stewards who don't use git opting out; work falling to one person; a broken event feed; a members list exposing someone.

### What we'll do

Each injection is a task under the Beads epic `sorr-l57` (relaunch the research group's output system). Proposed order, not yet worked through in a prerequisite tree: SoR team agreement, then the SoR /research page; the Substack rename and announcement; then the redirects, channel map and repo rules.

### Open questions

- Can stewards who don't use git work with this repo through agents, or do they need another surface?
- Does the SoR community count research as part of its funnel? This belongs to wider SoR strategy.

### Links

- [ltp/reason-commons.yaml](ltp/reason-commons.yaml): the trees
- [ltp/context.md](ltp/context.md): inputs, decisions and open questions
- [Purpose LTP](../../purpose-ltp/README.md): the research group's purpose (SCQ A)
