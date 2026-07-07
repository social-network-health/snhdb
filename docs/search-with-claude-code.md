# Search the SNH research library with Claude Code

*The local, fast replacement for the "Search with Claude Desktop + Google Drive" workflow.
Instead of an AI querying Google Drive over the network, you clone this repo once and an AI
searches the files on your own disk — card index first, then full papers.*

Status: **pilot — please run the test protocol below and record your timings.**
Old workflow for comparison:
[SNHDB Corpus Access via Google Drive](https://docs.google.com/document/d/1QlV5VQE1dEqhYEget6jJUSHRhCDfgrynyYdgXm6BoWU).

## One-time setup (~5 minutes)

1. **Install Claude Code** — https://claude.com/claude-code (`npm install -g @anthropic-ai/claude-code`,
   or download the desktop app). Sign in when prompted.
2. **Clone this repo** (needs ~1 GB free):
   ```sh
   git clone https://github.com/richbodo/snhdb.git
   cd snhdb
   ```
3. **Start Claude Code in the repo:**
   ```sh
   claude
   ```
   That's it. Claude reads this repo's `CLAUDE.md` automatically, which teaches it the
   two-stage search protocol (metadata cards first, then full-paper reading) and the
   corpus layout.

To update the library later: `git pull`.

### Optional: install the user-wide `/snhdb` skill

If you want to query the corpus from Claude Code sessions in *other* directories (e.g.
evidence-checking a claim in a document you're writing elsewhere):

```sh
mkdir -p ~/.claude/skills
ln -s ~/src/snhdb/skill/snhdb ~/.claude/skills/snhdb
```

Then, from any new Claude Code session: `/snhdb <your question>` — or just say "use the
snhdb skill to check whether this claim is supported." The skill locates the corpus
(`$SNHDB_PATH` → `~/src/snhdb` → a sibling checkout), freshens it with `git pull`, and
follows this repo's CLAUDE.md protocol. Tip: an allow rule for reading `~/src/snhdb` in
your Claude Code settings avoids per-session permission prompts.

## How to search

Just ask research questions in plain language, and ask for citations. Examples:

- *"What does this corpus say about loneliness interventions for remote workers? Cite the papers."*
- *"Which papers measure social isolation, and with what instruments?"*
- *"Summarize the evidence linking remote work to burnout. List the strongest 3 papers with DOIs and their limitations."*
- *"Find papers relevant to suicide-prevention program evaluation and give me each one's population and main claim."*

What good output looks like: paper titles + years + DOIs + repo file paths, claims traced
to the papers (not just to the metadata cards), and an honest "the corpus is thin here"
when it is.

Tip: if Claude reports nothing found, ask it to retry with broader vocabulary ("try
isolation, belonging, social support…") — the cards use research terms, not colloquial ones.

## The test protocol (please do this once)

We're measuring this workflow against the old Drive + Claude Desktop workflow. Run the same
three questions through **both** systems and record wall-clock time from pressing Enter to
having a **cited answer you'd act on** (not just a list of file names).

| # | Question | Drive + Claude Desktop | Claude Code + snhdb | Quality winner |
|---|---|---|---|---|
| 1 | "What does the research say about loneliness interventions for remote workers? Cite papers." | ___ min | ___ min | ___ |
| 2 | "Which papers in the corpus are about reaching hard-to-reach populations, and what methods do they use?" | ___ min | ___ min | ___ |
| 3 | "Summarize the evidence that remote work harms mental health — strongest 3 papers, with limitations." | ___ min | ___ min | ___ |

Also note, for each system:

- Did every cited paper actually exist? (spot-check one DOI)
- Did the answer draw on full papers or only on summaries/metadata?
- Anything the old system found that the new one missed (or vice versa)?

Mechanical baseline for reference: the card-index search step itself runs in ~10–20 ms on
this corpus (317 PDFs / ~1,300 markdown files) — total answer time is dominated by the AI
reading and writing, not by retrieval.

## Troubleshooting

- **"command not found: rg"** — Claude will fall back to `grep` on its own; answers are the
  same, slightly slower. (Optional: `brew install ripgrep`.)
- **Claude cites a paper twice with different paths** — it searched the legacy
  `Papers Data - Markdown Files Backup/` folder; tell it to exclude backups (CLAUDE.md
  already instructs this).
- **A paper has no markdown conversion** — some PDFs aren't converted yet; Claude should
  flag these rather than skip them. `rga` (ripgrep-all) can search inside PDFs if needed.
- **Permission prompts** — Claude Code asks before running shell commands; approving
  read-only search commands (`rg`, `ls`, `cat`) is safe and makes the session smoother.

## Why this is faster

The old path (Claude Desktop → MCP → Google Drive) pays a network round-trip for every
search *and* every document fetch, and Drive search can't see inside the YAML cards'
structure. Here the whole corpus is local: the card index answers "which papers?" in
milliseconds, and full papers stream off disk. The AI spends its time reading and
synthesizing — which is the part you actually want.
