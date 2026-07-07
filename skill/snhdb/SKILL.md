---
name: snhdb
description: Search the Social Network Health (SNH) research-paper corpus and answer research questions or evidence-check claims, with citations. Use when the user asks what the research or literature says about social network health, remote work, loneliness, isolation, social support, community health, burnout, or mental health; asks to verify whether a claim is supported by the SNH corpus; or invokes /snhdb with a question.
---

# snhdb — search the SNH research corpus

You are answering from **snhdb**, a local library of research papers (PDFs, full-text
markdown conversions, and YAML metadata cards). The user's question or claim-to-check is in
the arguments; if the arguments are empty, ask what they want to know.

## Step 1 — locate the corpus

Check in this order; use the first that exists (a directory containing `card-schema.yaml`):

1. `$SNHDB_PATH` (environment variable)
2. `~/src/snhdb`
3. `../snhdb` relative to the current repo root (sibling-checkout convention)

If none exists, tell the user the corpus isn't on this machine and ask before cloning
(it is ~1 GB): `git clone https://github.com/richbodo/snhdb.git ~/src/snhdb`.
If they decline, stop and point them at https://github.com/richbodo/snhdb.

## Step 2 — freshen (best-effort)

Only if the corpus checkout is clean and on its default branch
(`git -C <corpus> status --porcelain` empty), run `git -C <corpus> pull --ff-only` with a
short timeout. If it's dirty, on a work branch, offline, or diverged: skip, continue with
the local copy, and say so in one line — never block the answer on this.

## Step 3 — follow the corpus's own protocol

Read `<corpus>/CLAUDE.md` and follow its **two-stage search protocol exactly** (metadata
cards first with the documented exclusions, then whole-document reading of the markdown
conversions). That file is the canonical, maintained protocol — do not improvise a
different search strategy, and do not answer from cards alone.

## Step 4 — answer in the mode the user needs

- **Research question** → synthesize across the relevant papers. Cite each: title, year,
  DOI **confirmed from the full text** (card DOIs are unreliable), and the file path
  relative to the corpus root. Some conversions dropped the journal/DOI header — cite those
  as "DOI unverified in corpus copy" rather than trusting the card. Say honestly where the
  corpus is thin.
- **Claim check** (e.g. "is there evidence for the claim in section 1?") → first restate
  the claim precisely (read it from the user's document if they pointed at one), then
  report: **supported / contradicted / mixed / corpus is silent**, with the supporting or
  contradicting papers cited as above and a one-line note on evidence strength (design,
  sample, limitations — the cards' `claims[].support_strength` is a hint, the paper is the
  source).

Keep the final answer self-contained: someone who never sees the search steps should be
able to act on it and open every cited file.
