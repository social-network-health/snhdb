# snhdb

The **Social Network Health (SNH) research library**: a public collection of research
papers on social network health — remote work, loneliness and isolation, community health,
mental health, measurement methods — kept in one repository so anyone can clone it and
search the whole corpus **locally, in seconds**.

Each paper is stored three ways:

- the source **PDF** (`papers/<Topic>/`)
- a clean **full-text markdown conversion** (`papers/Markdown files/Papers_Data/<Topic>/MD/<paper>/`)
- a YAML **metadata card** — gist, claims, population, limitations, risk of bias —
  collected per topic in `<Topic>_Card_Schemas.md` files (format: `card-schema.yaml`)

The cards are the index; the papers are the source. AI tools search the cards in
milliseconds, then read the full papers before answering — no cloud storage round-trips,
no closed vector store.

## Intended usage

**1. Ask an AI, from anywhere on your machine (recommended).** Install the user-wide
`/snhdb` skill (below), then in any Claude Code session:

> `/snhdb What does the research say about loneliness interventions for remote workers? Cite papers.`
>
> *"Use the snhdb skill to check whether the claim in section 2 of this draft is supported by the evidence."*

**2. Ask an AI, inside this repo.** `cd snhdb && claude` — the repo's `CLAUDE.md` teaches
the session the search protocol automatically. Setup guide and a timed test protocol:
[`docs/search-with-claude-code.md`](docs/search-with-claude-code.md).

**3. Search by hand.** The corpus is plain files:

```sh
rg -i "your query" --glob "*Card_Schemas.md" --glob "!*Backup*" papers   # the card index
rga "your query" .                                                       # inside PDFs too
```

## Install

Needs ~1 GB free. Works on macOS and Linux (Windows: copy the folder instead of symlinking).

```sh
# 1. Get the library
git clone https://github.com/richbodo/snhdb.git ~/src/snhdb

# 2. Install the user-wide Claude Code skill (a symlink, so git pull updates it too)
mkdir -p ~/.claude/skills
ln -s ~/src/snhdb/skill/snhdb ~/.claude/skills/snhdb
```

Open a **new** Claude Code session anywhere and try `/snhdb <your question>`.

To update the library *and* the skill later:

```sh
git -C ~/src/snhdb pull
```

Prefer a different location? Clone anywhere and set `SNHDB_PATH=/path/to/snhdb` in your
environment — the skill checks it first.

## Contents & status

Papers are added periodically; organization and metadata are being actively cleaned up, so
expect the layout to evolve. Topics currently include Academic, Articles, Mental Health,
Remote Worker SNH, and Remote Workers. This repo will sync with the project's Google Drive
research folder and eventually power the AI search engine on
[toolkit.socialnetwork.health](https://toolkit.socialnetwork.health).

Part of the [Social Network Health Project](https://socialnetwork.health) ·
research hub: [social-network-health](https://github.com/richbodo/social-network-health)
