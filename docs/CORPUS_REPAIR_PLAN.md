# SNHDB Corpus Repair Plan

> **Status 2026-07-07:** all four decisions below approved by Rich; Phases 1 and 2
> are DONE (see "Repair log" at the bottom). Phase 3 (card regeneration) is next:
> pilot Remote Worker SNH with Fable-calibrated prompt, then fan out with Sonnet
> subagents + scripted validation gate; Fable spot-check QA on ~10-15%.

Companion to `docs/CORPUS_EVALUATION.md` (2026-07-07 audit). Ordered by
value-per-effort; each phase has concrete acceptance criteria measured by
re-running `tools/audit/`. Phases 1–2 are mostly scriptable; Phase 3 is the
substantive rebuild.

## Decisions needed before executing (please confirm/override)

1. **Source of truth for cards.** Proposal: the per-paper
   `MD/<paper>/card_schema.md` is canonical; the combined
   `*_Card_Schemas.md` files are **generated** from them by a script
   (`tools/audit/build_combined_cards.py`, to be written). Today the two are
   out of sync and nothing declares which wins.
2. **Duplicates policy.** Proposal: keep the copy in the most specific topic
   folder, delete `(1)`/`(2)`/`(Duplicate)`/`.pdf.pdf` copies and the
   cross-topic Schaufeli duplicate, and record removals in a `DUPLICATES.md`
   ledger so Drive sync doesn't resurrect them.
3. **Backup dir.** `papers/Papers Data - Markdown Files Backup/` stays frozen
   (excluded from all tooling) until Phase 3 is verified, then gets deleted.
4. **No-DOI marking.** Extend `card-schema.yaml` so `doi: null` is
   disambiguated by `source.notes: "no-doi: <reason>"` (e.g. blog post,
   report). Alternative: a new `doi_status:` field — schema change, your call.

## Phase 1 — File hygiene (scriptable, ~an hour, low risk)

Fixes the structural rot so later phases key off clean names.

- Rename `*.pdf.pdf` → `.pdf`; delete the two stray PDFs inside the MD tree.
- Strip trailing spaces (and normalize unicode dashes where they break card
  links) from conversion folder names; fix affected `source.markdown` paths.
- Re-download the corrupt UyBico 2007 PDF; convert it.
- Deduplicate PDFs and conversion folders per decision #2.
- Remove the stray `Source Word file:` footer from the 5 combined card files.
- Re-convert `World Health Statistics 2023` without the 50-page cap (or
  explicitly mark the card "excerpt: first 50 pages").
- Decide fate of the two near-empty conversions (spreadsheet, Reddit thread):
  re-convert properly or mark as stubs.

**Acceptance:** `analyze.py` reports 0 unconverted_pdf (except deliberate),
0 duplicate_pdf, 0 orphan_conversion, 0 card_without_conversion caused by
path issues.

## Phase 2 — DOI repair (mostly automatable, highest value/effort)

Work from `tools/audit/out/doi_verdicts.json`:

1. **15 unresolvable DOIs** — typos/truncations. Crossref bibliographic search
   on the paper title; auto-accept when returned title similarity ≥ 0.9, queue
   the rest for eyeball.
2. **47 wrong-paper DOIs** — same treatment: title-search Crossref, replace,
   verify. These are reference-list captures; never trust the in-text DOI again
   without a title match.
3. **7 borderline** — manual review (list is in doi_verdicts.json).
4. **77 missing DOIs with confident suggestions** — apply after the same ≥ 0.9
   title check; spot-check 10 by hand before bulk-applying.
5. **~75 remaining no-DOI cards** — classify: blog/industry article (mark
   per decision #4) vs academic paper needing manual lookup.

Invariant going forward: **a DOI is written to a card only if Crossref's
registered title matches the paper title.** The checker already exists
(`crossref_check.py`); the apply-script (`tools/audit/apply_doi_fixes.py`)
needs writing.

While applying, also backfill `authors`, `year`, `venue`, and `citation` from
the Crossref record — this mechanically fixes most of the 77 bad-author cards
and the junk venues for every paper that ends up with a verified DOI.

**Acceptance:** re-run `crossref_check.py`: 0 unresolvable, 0 wrong-paper;
every remaining `doi: null` carries an explicit no-DOI reason.

## Phase 3 — Card regeneration (the substantive rebuild)

The gists, claims, tags, and population blocks are templated noise; they must
be **regenerated from the full-text markdown**, not patched. Proposal:

- Batch job (Claude, topic-by-topic, ~320 papers): read
  `MD/<paper>/<paper>.md`, produce a fresh card per `card-schema.yaml` —
  slug `id`, real paper `title` from the title block, genuine 2–3 sentence
  `gist`, 2–3 **findings** (not aims) as claims with per-claim
  `outcomes`/`predictors` chosen from the controlled vocabulary, real
  population block, paper-specific `relevance_to_project`, honest
  `risk_of_bias`.
- Metadata fields (`authors`, `year`, `doi`, `venue`, `citation`) come from
  Phase 2's Crossref-verified record, not from the LLM — the model only writes
  the fields that require reading the paper.
- **Validation gate per card** (script): YAML parses; required fields present;
  `id` is slug-format and unique; gist doesn't match the old template; claims
  are non-identical and tag lists differ across claims where the paper
  supports it; `source.markdown` resolves.
- Human QA: sample ~10 cards per topic (~15% of corpus) against the papers
  before accepting a topic batch.
- Regenerate the combined `*_Card_Schemas.md` from the accepted individual
  cards (decision #1), then update `CLAUDE.md` pitfalls that no longer apply.

Sequencing suggestion: start with **Remote Worker SNH** (16 cards — smallest,
core topic) to shake out the prompt and validation gate, then Mental Health,
Academic, Articles, Remote Workers (150).

**Acceptance:** `analyze.py` reports 0 boilerplate_gist/relevance, 0
bad_authors, 0 title_is_filename, 0 raw_doi_id, 0 duplicate_card_title;
sampled-card QA passes.

## Phase 4 — Source retrieval + conversion touch-ups (checklist, 2026-07-08)

**Rich (needs logins / a real browser). Save each file over the existing path,
then tell the agent so it re-converts and regenerates the card:**

- [x] **UyBico 2007 PDF** (done 2026-07-08: retrieved by Rich via PMC, converted, carded) — open https://pmc.ncbi.nlm.nih.gov/articles/PMC2219860/
      and click "PDF (251.6 KB)". Save over
      `papers/Remote Worker SNH/UyBico et al 2007 - Recruiting Vulnerable Populations into Research.pdf`
      (current file is a saved Springer bot-wall HTML page). Springer original
      (paywalled): https://doi.org/10.1007/s11606-007-0126-3
- [x] **Workplace Isolation dissertation (full text)** (done 2026-07-08: full 141-page PDF retrieved by Rich, converted, card regenerated) — the corpus PDF is a
      24-page capture (front matter + ch. 1 only). Full citation: Adam Hickman,
      "Workplace Isolation Occurring in Remote Workers", PhD dissertation,
      Walden University, May 2019. Find via
      https://scholar.google.com/scholar?q=%22Workplace+Isolation+Occurring+in+Remote+Workers%22+Hickman
      or https://scholarworks.waldenu.edu/do/search/?q=%22Workplace+Isolation+Occurring+in+Remote+Workers%22
      Save over `papers/Remote Workers/Workplace Isolation Occurring in Remote Workers.pdf`.
- [x] **Rust Reddit thread** (done 2026-07-08: identified as the r/Redox ny8d1j thread discussing the Soller post; captured via browser; folder renamed "...Redox Community"; login-wall PDF removed, markdown-only source) — the capture is Reddit's login-wall page and the
      original URL was not preserved. While logged in to Reddit, find the thread
      (try https://www.google.com/search?q=site%3Areddit.com+rust+%22open+source%22+%22mental+health%22 )
      and print-to-PDF over
      `papers/Articles/Open Source and Mental Health Reddit Discussion Rust Community.pdf`.
- [x] **HBR "A Study of 1,100 Employees…" (Grenny & Maxfield 2017)** (done 2026-07-08: full 6-page PDF from Rich's HBR account; converted + re-carded — prior capture was summary-only)
      — current conversion holds only the summary (~200 words). Needs HBR access:
      https://hbr.org/2017/11/a-study-of-1100-employees-found-that-remote-workers-feel-shunned-and-left-out
- [ ] *(optional)* **"Open Source Articles Research Spreadsheet"** — conversion is
      a 372-char stub of a spreadsheet; re-export the source sheet (or drop it).

**Agent (no logins needed):**

- [x] Re-convert `World Health Statistics 2023` in full (done 2026-07-08: pdftotext conversion, all 136 pages, card regenerated) — the PDF is complete
      (136 pages); only the conversion stopped at 50.
- [x] Re-convert + regenerate cards for each document Rich retrieves above (done 2026-07-08)
      (mini-pipeline: convert → gen agent → assemble → build_combined_cards).
- [x] Verify "How I Recognize And Prevent Burnout In Open Source" — confirmed complete (image-heavy page; article footer present)
      is content-complete (likely just image-heavy), then close it out.
- [x] Delete the AI-generated Vorecol marketing blog post (done 2026-07-08,
      recorded in DUPLICATES.md; Remote Workers now 131 cards).

## Phase 5 — Guardrails so it stays fixed

- Keep `tools/audit/` as the standing corpus health check; run it before any
  Google Drive sync or toolkit.socialnetwork.health ingestion. Optionally add a
  `make audit` target and commit `out/` summaries (not the bulky manifest).
- Intake rule for new papers: conversion + card + Crossref-verified DOI +
  audit pass before a paper counts as "in the corpus".
- After Phase 3, delete the Backup dir (decision #3) and simplify the
  CLAUDE.md pitfall list to match the repaired reality.

## Effort estimate

| Phase | Mode | Rough effort |
|---|---|---|
| 1 File hygiene | script + review | 1–2 h |
| 2 DOI repair | script + ~30 manual lookups | 2–4 h |
| 3 Card regeneration | LLM batch + validation + QA | the bulk; 1–2 sessions per topic |
| 4 Conversion touch-ups | manual, 5 files | 1 h |
| 5 Guardrails | script/docs | 1 h |

## Repair log

### 2026-07-07 — Phase 1 (file hygiene) DONE
- Deduplicated 24 duplicate PDFs (17 hash-identical groups + same-paper
  re-downloads) and their 22 duplicate conversion folders; ledger in
  `DUPLICATES.md`. Corpus: 317 → 289 PDFs, 316 → 294 conversions.
- Fixed `.pdf.pdf` double extensions (Dingel & Neiman; Podsakoff duplicate
  deleted); renamed 2 trailing-space folders; repointed 6 drifted
  `source.markdown` paths (all card source paths now resolve).
- UyBico 2007: the "PDF" was a saved Springer bot-wall HTML page. Real PDF is
  paywalled at Springer; the PMC author manuscript (PMC2219860) is open but
  bot-gated — **pending manual download** (see plan Phase 4 note).
- Known leftovers: World Health Statistics 2023 page-cap re-conversion and the
  2 near-empty conversions (deferred to Phase 4 as planned).

### 2026-07-07 — Phase 2 (DOI repair + metadata backfill) DONE
- Every one of 294 cards now has a decided DOI status
  (`tools/audit/out/verified_metadata.json`):
  210 kept/auto-verified · 82 newly resolved · 45 wrong DOIs replaced ·
  29 manually adjudicated (incl. JSTOR review DOIs from stable URLs, and the
  DataCite-registered Hooper 2008) · 55 confirmed no-DOI with reason written
  to `source.notes` (blogs, HBR pieces, dissertations, reports, newsletters).
- Rule enforced: a DOI is only written when the registry's title matches the
  paper (Crossref ≥0.9 similarity, or human check). authors/year/venue/citation
  and slug `id` backfilled from the verified record on all matched cards.
- Combined `*_Card_Schemas.md` files are now GENERATED from per-paper cards
  (`tools/audit/build_combined_cards.py`); 294 cards = 294 conversions, 0 YAML
  parse errors.
- Mislabeled-content folders discovered (fix titles in Phase 3 QA): the
  "Gladwin (1981) Culture's Consequences review" folder actually contains
  Andrews' review of Burt's *Structural Holes* (card metadata now reflects the
  actual content); "Brayfield & Rothe (1951)" markdown begins with a fragment
  of the preceding journal piece.

### 2026-07-07 — Phase 3 (card regeneration) DONE
- All 294 cards regenerated from full-text markdown. Pipeline:
  `gen_payloads.py` → one Sonnet agent per paper (Workflow fan-out; pilot topic
  Remote Worker SNH QA'd first) → `assemble_cards.py` validation gate (enum,
  anti-boilerplate, length, YAML round-trip) → combined files regenerated.
  Bibliographic fields came from Phase 2's Crossref-verified records, never the LLM.
- Acceptance met: 0 templated gists (was 319), 0 boilerplate relevance strings,
  0 raw-DOI ids, 0 card parse errors, 294 cards = 294 conversions.
- Fidelity screen (`check_claim_fidelity.py`): of 247 cards with numeric claims,
  218 have every number verbatim in the source; all 8 below-threshold cases were
  hand-verified as formatting artifacts (spelled-out numbers, Lancet middle-dot
  decimals), not fabrication. Manual QA: Wingman-Connect RCT effect sizes,
  O'Hare regression coefficients, Developer Crisis / Maintainer Squeeze
  percentages all confirmed against sources.
- Fixed en route: a staging-filename collision that had cross-contaminated the
  Good Behavior Game main-paper/editorial card pair (regenerated both).
- New Phase 4 items surfaced by generation agents: `Workplace Isolation
  Occurring in Remote Workers` dissertation markdown truncated after chapter 1;
  the Reddit-thread source is a login-wall stub; one Remote Workers source is an
  AI-generated marketing blog post (card marks it high risk-of-bias) — consider
  whether it belongs in the corpus at all.
- Cost note: ~13.5M Sonnet tokens for 296 agents (~45k/paper), per the approved
  Sonnet-for-volume / Fable-for-QA split.

### 2026-07-08 — Phase 4 essentially DONE
Rich retrieved UyBico 2007 (PMC) and the full 141-page Workplace Isolation dissertation;
agent converted both (pdftotext; note: plainer than Marker output) plus full WHS 2023,
regenerated all three cards, captured the r/Redox mental-health thread via browser
(login-wall PDF removed; folder renamed Redox Community), and removed the AI-generated
Vorecol blog post. Staging filenames now use stable card-path hashes. Remaining optional:
HBR "1,100 Employees" full text (needs HBR sub) and the research-spreadsheet stub.
Related deliverable: proposed check-in protocol design note written to
social-network-health/research/protocols/checkin_protocol.md (v0.1, open questions listed).

### 2026-07-08 (later) — HBR additions
- "A Study of 1,100 Employees…" full text installed and re-carded.
- NEW source added: Ponte 2022, "How to Be a Mental Health Ally" (HBR) →
  `papers/Mental Health/How to Be a Mental Health Ally - HBR 2022.pdf`. NOTE: the
  PDF export is a partial capture (summary + opening paragraph + bio; hbr.org
  shows "reserved for Subscribers" when not logged in in this browser profile).
  Card marks the partial capture; re-export while logged in to HBR and drop in
  /incoming to complete it. Corpus now 295 cards = 295 conversions, audit green.

### 2026-07-08 (later still) — Ponte 2022 completed; Backup dir deleted
- "How to Be a Mental Health Ally" full 13-page PDF re-exported by Rich while
  logged in; converted and card regenerated from full text (earlier export had
  silently truncated at the subscriber wall).
- `papers/Papers Data - Markdown Files Backup/` (35 MB legacy duplicate)
  deleted per decision #3 — Phase 3 cards verified by Rich.
- Diagnosed the last optional item: `Open Source Articles Research
  Spreadsheet.pdf` is a Pdfcrowd capture of the **Google Sheets sign-in page**
  (same login-wall failure mode as the old Reddit/UyBico captures). The real
  source is a Google Sheet in the Drive research folder. Options: export it
  (File → Download → PDF/CSV) into /incoming to be converted+carded, or drop
  it from the corpus if it was only an internal tracking index. Awaiting
  Rich's call.
