# CLAUDE.md

This file teaches Claude Code (claude.ai/code) how to work in this repository.

## What this repo is

**snhdb** — the Social Network Health (SNH) research-paper library: ~300+ papers as PDFs,
markdown conversions of most of them, and YAML **metadata cards** summarizing each paper
(gist, claims, population, limitations, risk of bias). It exists so a human with Claude Code
can search the whole corpus locally, in seconds, instead of querying Google Drive.

Your job in most sessions: **answer research questions from the corpus, with citations.**

## Layout

```
card-schema.yaml                      the card format spec (field meanings live here)
papers/<Topic>/*.pdf                  the source PDFs, by topic
papers/Markdown files/Papers_Data/<Topic>/
    <Topic>_Card_Schemas.md           ALL cards for that topic, one file  ← search these first
    MD/<paper-name>/
        <paper-name>.md               full-text markdown conversion       ← then read these
        <paper-name>_meta.json        conversion metadata
        card_schema.md                that paper's individual card
        _page_*.jpeg                  extracted figures (usually ignore)
docs/, uncategorized/                 intake notes and not-yet-filed material
```

Topics currently: Academic · Articles · Mental Health · Remote Worker SNH · Remote Workers
(plus `Summery Files` [sic] and `Writings` under Papers_Data). **The organization is being
actively cleaned up — verify paths with `ls` rather than assuming this map is current.**

## The search protocol (two stages — follow this)

**Stage 1 — cards first.** Search the combined card files, excluding the legacy backup:

```
rg -i "<term>" --glob "*Card_Schemas.md" --glob "!*Backup*" papers
```

Cards are YAML: match against `gist`, `claims[].text`, and the controlled-vocabulary tags
`outcomes:` / `predictors:` (e.g. `outcomes: ["turnover", "collaboration"]`). Pull each hit's
`title:`, `id:` (DOI), and `relevance_to_project:` with a few lines of context (`-B6 -A6`).

**Vocabulary matters more than cleverness.** The cards use research vocabulary, not
colloquial phrasing — e.g. "help-seeking" gets zero card hits while "isolation" gets
hundreds. Expand every question into 3–6 alternative terms (isolation, loneliness, social
support, belonging, intervention, wellbeing, burnout, turnover…) before concluding the
corpus is silent.

**Stage 2 — read the papers.** For the 3–10 most relevant cards, open the full-text
conversion at `papers/Markdown files/Papers_Data/<Topic>/MD/<paper-name>/<paper-name>.md`
and read whole documents (they are clean markdown, typically a few hundred lines). Do NOT
answer from cards alone when the question needs evidence detail — the card is the index,
the paper is the source.

**Cite** every claim: paper title, year, DOI (the card's `id:`), and the repo-relative file
path so the human can open it.

## Pitfalls

- `papers/Papers Data - Markdown Files Backup/` is a **legacy duplicate** — always exclude
  it (`--glob "!*Backup*"`) or you will double-count papers. (Scheduled for deletion.)
- Directory names contain spaces and punctuation (`&`, parentheses) — quote paths in shell
  commands.
- Cards' `source.markdown` values are prefixed `Papers_Data/…` but the files live under
  `papers/Markdown files/Papers_Data/…` — prepend the missing segment when resolving.
- A handful of sources are not papers (blog posts, HBR pieces, dissertations, reports,
  one whole journal issue). Their cards say so: `doi: null` plus a `source.notes`
  beginning `no-doi:` explaining why. `risk_of_bias`/`support_strength` reflect that.
- Known damaged conversions (fix pending, see docs/CORPUS_REPAIR_PLAN.md Phase 4):
  `World Health Statistics 2023` (first 50 of 136 pages), `Workplace Isolation Occurring
  in Remote Workers` (dissertation truncated after ch. 1), the Reddit-thread stub (login
  wall only), and the corrupt UyBico 2007 PDF.
- The same paper occasionally appears in two topic folders (e.g. the Wyman 2019
  peer-adult network paper, Wingman-Connect) — cite it once.

**Card trust status (since the 2026-07 repair):** cards were regenerated from full text
with Crossref-verified bibliographic metadata. `doi`, `authors`, `year`, `venue`,
`citation` are verified (see `tools/audit/out/verified_metadata.json`); `gist`, `claims`,
`population`, `limitation`, `relevance_to_project` were written by an LLM reading the
full markdown, behind a validation gate plus a numeric-fidelity screen. For high-stakes
citations still confirm the claim in the full text — the card tells you where to look.

## Corpus health checks

`tools/audit/` is the standing audit harness (needs brew poppler + python pyyaml):
`build_manifest.py` → `analyze.py` (inventory + issue counts), `crossref_check.py`
(DOI verification), `check_claim_fidelity.py` (claim numbers vs source text). The
combined `*_Card_Schemas.md` files are **generated** — never edit them by hand; edit the
per-paper `MD/<paper>/card_schema.md` and run `build_combined_cards.py`. Run the audit
before any Drive sync or toolkit.socialnetwork.health ingestion.

## Conventions for changes

- Card format changes go through `card-schema.yaml` (its header comment states formatting
  rules: double-quoted scalars, flow-style `venue`/`method`, one `#` heading per card file).
- This corpus will sync with the Google Drive research folder and eventually power the
  toolkit.socialnetwork.health search engine — don't restructure directories without asking.
- Related project map: `social-network-health` repo (sibling checkout) → `RELATED_REPOS.md`.
