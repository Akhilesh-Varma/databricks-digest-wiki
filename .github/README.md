# Daily Databricks Digest — Knowledge Wiki

> An auto-generated knowledge graph of every story aired on the *Daily Databricks Digest* podcast. Updated daily.

[![Deploy status](https://github.com/Akhilesh-Varma/databricks-digest-wiki/actions/workflows/deploy.yml/badge.svg)](https://github.com/Akhilesh-Varma/databricks-digest-wiki/actions/workflows/deploy.yml)

🌐 **Live website:** **<https://akhilesh-varma.github.io/databricks-digest-wiki/>**
🎙️ **Listen to the podcast on Spotify:** **https://open.spotify.com/show/0o8UdVTvUVaNmcoxzgQ0zU**

---

## Table of contents

- [What is this?](#what-is-this)
- [Two ways to read this wiki](#two-ways-to-read-this-wiki)
- [Browse in your browser (easy)](#browse-in-your-browser-recommended)
- [Open in Obsidian (recommended)](#open-in-obsidian-advanced)
- [Repository layout](#repository-layout)
- [Page types and frontmatter reference](#page-types-and-frontmatter-reference)
- [Where to start? Reading paths](#where-to-start-reading-paths)
- [How the wiki is generated](#how-the-wiki-is-generated)
- [About the podcast](#about-the-podcast)
- [Content disclaimer](#content-disclaimer)
- [Reporting errors or requesting takedowns](#reporting-errors-or-requesting-takedowns)
- [License](#license)

---

## What is this?

This repository is the Markdown vault behind the **Daily Databricks Digest Wiki** — a continuously-growing reference that mirrors, in written form, every story discussed on the *Daily Databricks Digest* podcast. Each weekday morning at 6 AM EST, an automated pipeline:

1. Surfaces the day's most relevant Databricks, lakehouse, and data-engineering stories from public sources
2. Generates the day's podcast script and audio
3. Extracts entities — companies, technical concepts, people — from each story using a cascade of LLMs (Claude → Gemini → Groq Llama)
4. Writes the result to this repo as Obsidian-compatible Markdown plus a `graph.json` knowledge-graph dump
5. Triggers a GitHub Actions workflow that builds and publishes the public website

The output is two complementary artifacts that pair with the audio:

- A **public website** — search, dark mode, interactive graph, no setup
- An **Obsidian vault** (this repo) — local-first, full backlinks, works offline, supports your own annotations alongside

If you've heard the podcast and wanted a written, link-rich reference for what was discussed, this is it.

---

## Two ways to read this wiki

| | 🌐 Browser | 📒 Obsidian |
|---|---|---|
| **Setup time** | None | ~3 minutes |
| **Search** | ✓ | ✓ |
| **Graph view** | ✓ | ✓ (richer, plugin ecosystem) |
| **Backlinks panel** | Limited | ✓ |
| **Add your own notes** | ✗ | ✓ |
| **Works offline** | ✗ | ✓ |
| **Mobile** | ✓ | ✓ (Obsidian mobile) |
| **Best for** | Quick reference, casual reading, sharing | Power users, researchers, building on top |

---

## Browse in your browser (easy)

Just visit **<https://akhilesh-varma.github.io/databricks-digest-wiki/>** — no install, no clone, no Obsidian.

You get:

- 🔍 **Full-text search** across every story, entity, and episode
- 🌐 **Interactive graph view** of all connections (concepts ↔ companies ↔ episodes ↔ stories)
- 🌓 **Dark mode toggle**
- 📱 **Mobile-friendly layout**
- 🔗 **Click any entity** to see every story where it's mentioned, and every other entity it connects to

The site rebuilds within ~3 minutes of every wiki update, so what you see on the website is never more than one cycle behind this repository.

---

## Open in Obsidian (recommended)

For richer linking, offline access, and the ability to annotate the auto-generated content with your own notes.

### Prerequisites

- **Obsidian** — free download at <https://obsidian.md>
- **Git** — to keep your local vault current

### Setup

1. **Clone this repository** to a location on your machine where you keep Obsidian vaults:

   ```bash
   git clone https://github.com/Akhilesh-Varma/databricks-digest-wiki.git ~/Obsidian/databricks-digest-wiki
   ```

   (Replace `~/Obsidian/databricks-digest-wiki` with whatever path you prefer.)

2. **Open it in Obsidian:**
   - Launch Obsidian
   - Click **"Open another vault"** (the bottom-left icon on the home screen)
   - Choose **"Open folder as vault"**
   - Pick the folder you just cloned
   - Trust the vault when prompted

3. **Recommended Obsidian settings** (Settings → Editor / Files & Links / Appearance):
   - **Files & Links** → **New link format**: *Shortest path when possible* (matches how the auto-generated content links)
   - **Files & Links** → **Use [[Wikilinks]]**: enabled
   - **Editor** → **Show frontmatter**: enabled (frontmatter holds metadata like episode date, source URL, extraction model)
   - **Appearance**: pick any theme — the auto-generated content is theme-agnostic

4. **Suggested community plugins** (Settings → Community plugins → Browse):
   - **Graph Analysis** — extends the default graph view with PageRank, centrality, and other useful metrics
   - **Dataview** — query frontmatter to build custom indexes (e.g. "all stories where Databricks is the main subject," "all concepts mentioned in the last week")
   - **Tag Wrangler** — manage the auto-generated `#story`, `#concept`, `#company`, `#person`, `#episode` tags

### Updating

The repository is rewritten by the automated pipeline once per weekday morning. To pull the latest content into your local vault:

```bash
cd ~/Obsidian/databricks-digest-wiki
git pull
```

You can keep your own notes alongside the auto-generated ones — just keep them in folders that don't conflict with the auto-managed ones (`episodes/`, `sources/`, `companies/`, `concepts/`, `people/`). For example, in a `_my-notes/` directory at the root. Files outside the auto-managed folders are never touched by the pipeline.

> ⚠️ **Heads-up about merge conflicts:** the pipeline uses a mirror-style sync that fully replaces the auto-managed folders on every run. If you edit auto-generated files in place, your edits will be overwritten on the next sync. For personal annotations, prefer creating *sibling* notes in `_my-notes/` and using backlinks (`[[concepts/iceberg|Iceberg]]`) to reference the auto-generated entries.

---

## Repository layout

```
.
├── index.md              ← Landing page (rendered as the homepage on the website)
├── episodes/             ← One Markdown file per podcast episode
│   └── 2026-05-06.md
├── sources/              ← One file per news story aired in episodes
│   └── 2026-05-06/
│       └── 01_apache-iceberg-on-databricks.md
├── companies/            ← Auto-extracted company entities, with backlinks to every story
│   └── databricks.md
├── concepts/             ← Auto-extracted technical concepts (Lakehouse, Iceberg, RBAC, …)
│   └── unity-catalog.md
├── people/               ← Auto-extracted people (hidden from the public website by default)
├── graph.json            ← Full knowledge-graph dump: nodes + edges
└── .github/
    ├── workflows/
    │   └── deploy.yml          ← Builds the website with Quartz on every push to main
    ├── quartz/
    │   ├── quartz.config.ts    ← Site config override (title, theme, ignored paths)
    │   └── disclaimer.md       ← Per-page disclaimer banner content
    └── README.md               ← This file
```

Every Markdown page has YAML frontmatter capturing the page type, source URL, extraction model, content hash, and timestamps — useful both for human readers and as machine-readable metadata for tools like Dataview.

### Conventions

**Tags.** Auto-applied tags identify page type and source feed. Filter by tag in Obsidian via the Tags pane, or with Dataview queries.

| Tag | Applied to |
|---|---|
| `#episode` | Episode hub pages under `episodes/` |
| `#story` | Individual story pages under `sources/` |
| `#concept` | Concept entity pages under `concepts/` |
| `#company` | Company entity pages under `companies/` |
| `#person` | Person entity pages under `people/` |
| `#source/reddit`, `#source/rss`, `#source/devto`, `#source/github_releases`, `#source/databricks_community`, `#source/hackernews` | Story pages — which feed produced the article |

**Wikilink format.** Pages cross-reference each other using Obsidian-style wikilinks. The pipe character separates the file path from the display label.

```markdown
[[concepts/iceberg|Iceberg]]
[[episodes/2026-05-06]]
[[sources/2026-05-06/01_apache-iceberg-on-databricks|This story]]
```

Quartz on the website renders these as regular HTML links; Obsidian renders them as backlinked Markdown with the target highlighted on hover.

**Filename patterns.** Slugs are deterministic — the same entity always gets the same slug, so backlinks stay stable across rebuilds.

| Pattern | Example |
|---|---|
| `episodes/YYYY-MM-DD.md` | `episodes/2026-05-06.md` |
| `sources/YYYY-MM-DD/<rank>_<slug>.md` | `sources/2026-05-06/01_apache-iceberg.md` |
| `companies/<slug>.md` | `companies/databricks.md` |
| `concepts/<slug>.md` | `concepts/unity-catalog.md` |
| `people/<slug>.md` | `people/matei-zaharia.md` |

`slugify()` lowercases, kebab-cases, and strips diacritics. The leading rank in story filenames (01, 02, …) corresponds to that story's position in the episode (01 = opening / top story).

---

## Page types and frontmatter reference

Each kind of page has a consistent frontmatter shape. Knowing the fields lets you query the vault programmatically (Dataview), spot stale content, or audit the LLM extraction.

### `episodes/<YYYY-MM-DD>.md` — episode hub

The aggregate page for one day's podcast episode. Links to every story aired and lists every concept covered.

| Field | Type | Description |
|---|---|---|
| `type` | `"episode"` | Page-type discriminator |
| `episode_date` | date | YYYY-MM-DD, matches the filename |
| `title` | string | Human-readable episode title |
| `duration_seconds` | int | Length of the audio file |
| `audio_url` | string | Direct link to the episode's |
| `provider` | string | Which provider generated the script (audit trail) |
| `story_count` | int | Number of stories in this episode |
| `tags` | array | `[episode]` |

**Body:** ordered list of stories aired (linked via wikilinks), followed by a flat list of every concept covered.

### `sources/<YYYY-MM-DD>/<rank>_<slug>.md` — story page

The atomic unit of the wiki. One file per news article that aired in an episode.

| Field | Type | Description |
|---|---|---|
| `type` | `"story"` | Page-type discriminator |
| `story_id` | string | Stable ID across pipeline reruns |
| `episode_date` | date | The episode this story aired in |
| `rank` | int | Position in that episode (1 = top story) |
| `source` | string | Which feed produced this article (`reddit`, `rss`, `devto`, `github_releases`, `databricks_community`, `hackernews`) |
| `url` | string | Original article URL |
| `title` | string | Article title |
| `quality_score` | float | Internal ranking score, 0-1 |
| `content_hash` | string | SHA-256 of the article body (cache invalidation) |
| `concepts`, `companies`, `people` | array of slugs | Extracted entities |
| `extractor_model` | string | Which LLM produced the extraction (e.g. `claude-sonnet-4-6`, `gemini-2.5-flash-lite`, `llama-3.3-70b-versatile`) |
| `extracted_at` | timestamp | When extraction ran |
| `tags` | array | `[story, source/<feed-name>]` |

**Body:** summary (3-5 sentences), key claims (bullets), source URL, then a "Related" section linking to every entity mentioned.

### `companies/<slug>.md` — company entity

Aggregation page for a company referenced in any story.

| Field | Type | Description |
|---|---|---|
| `type` | `"company"` | Page-type discriminator |
| `name` | string | Display name |
| `slug` | string | URL-safe identifier (matches filename) |
| `first_seen` | date | First episode that mentioned this company |
| `last_seen` | date | Most recent episode |
| `mention_count` | int | Total mentions across all stories |
| `avg_confidence` | float \| `""` | Average extractor confidence (sometimes empty for legacy entries) |
| `tags` | array | `[company]` |

**Body:** mention-count blurb, then "Appears in" — every story grouped by episode date.

### `concepts/<slug>.md` — concept entity

Same shape as `companies`, with `type: "concept"` and `tags: [concept]`. Concepts include things like `unity-catalog`, `apache-iceberg`, `lakehouse`, `delta`, `rest-api`, `rbac`.

### `people/<slug>.md` — person entity

Same shape with `type: "person"` and `tags: [person]`.

> **Hidden from the public website.** Person entity extraction is the noisiest layer of the pipeline (first-name-only matches, occasional cross-contamination with off-topic articles). Until extraction quality is validated, person pages are excluded from the published site via the [`ignorePatterns`](.github/quartz/quartz.config.ts) override. They remain in the cloned vault for personal use.

### `index.md` — landing page

The homepage. Lists recent episodes (newest first) and top concepts ranked by mention count.

| Field | Type | Description |
|---|---|---|
| `type` | `"index"` | |
| `generated_at` | timestamp | When the index was last rebuilt |
| `episode_count` | int | Total episodes covered |
| `story_count` | int | Total stories indexed |

### `graph.json` — knowledge-graph dump

Machine-readable JSON representation of the full wiki, useful for programmatic analysis (network science, custom visualizations, ML).

```json
{
  "episodes": [{"episode_date": "2026-05-06", "title": "...", "story_count": 10}],
  "stories":  [{"story_id": "...", "title": "...", "episode_date": "...", "rank": 1, "quality_score": 0.85}],
  "entities": [{"kind": "concept|company|person", "slug": "...", "name": "...", "mention_count": 42}],
  "edges": [
    ["story/<id>", "episode/<date>", "aired_in"],
    ["story/<id>", "concept/<slug>", "mentions"],
    ["story/<id>", "company/<slug>", "mentions"],
    ["story/<id>", "person/<slug>",  "mentions"]
  ]
}
```

Load it into NetworkX, Neo4j, or your favorite graph tool to run custom analyses.

---

## Where to start? Reading paths

Different goals → different entry points.

### 🎧 Casual listener — "what was on yesterday's episode?"

1. Open the [website](https://akhilesh-varma.github.io/databricks-digest-wiki/) (or `index.md` in Obsidian)
2. Click the most recent episode under "Recent episodes"
3. Read the story summaries; click into any source for the full LLM extraction
4. Each story page links back to the original article URL — go read the original if you want depth

### 🔬 Researcher — "what's been said about Iceberg recently?"

1. Search for "iceberg" using the website's search bar (or Obsidian's `Cmd/Ctrl + O`)
2. Land on `concepts/iceberg.md` — the aggregation page lists every story that mentioned the concept
3. Each entry links to the source URL and the relevant episode page
4. Sort by `last_seen` or `mention_count` in the frontmatter to see what's trending

### 🛠 Developer — "I want to do graph queries on this"

1. Pull `graph.json` from the repo (raw URL: <https://raw.githubusercontent.com/Akhilesh-Varma/databricks-digest-wiki/main/graph.json>)
2. Load it into NetworkX, Neo4j, or your tool of choice — the schema is documented in the [Page types reference](#page-types-and-frontmatter-reference) above
3. Or query the Markdown frontmatter directly using Dataview if you've cloned the vault into Obsidian

### 📒 Power user — "I want to layer my own notes on top"

1. Clone the repo as an Obsidian vault (see [Open in Obsidian](#open-in-obsidian-advanced))
2. Create `_my-notes/` at the root for your own files — anything outside the auto-managed folders is never touched by the pipeline
3. Use wikilinks `[[concepts/iceberg|Iceberg]]` in your notes to backlink to auto-generated pages — those backlinks then surface in the auto-generated page's "Linked mentions" panel in Obsidian, so your annotations are discoverable from both sides

---

## How the wiki is generated

```
┌──────────────────────────────────────────────────────────────────┐
│ Public news sources                                              │
│  Reddit • RSS • Hacker News • Databricks Community • dev.to …   │
└──────────────────────────────┬───────────────────────────────────┘
                               ▼
┌──────────────────────────────────────────────────────────────────┐
│ Databricks pipeline (private repo)                               │
│  Bronze ingestion → Silver cleaning → Gold ranking & dedup      │
│  Top stories per day selected via quality scoring                │
└──────────────────────────────┬───────────────────────────────────┘
                               ▼
┌──────────────────────────────────────────────────────────────────┐
│ LLM extraction cascade (Anthropic Claude → Google Gemini → Groq) │
│  • Story summary                                                 │
│  • Key claims                                                    │
│  • Technical concepts (with confidence scores)                   │
│  • Companies and people                                          │
└──────────────────────────────┬───────────────────────────────────┘
                               ▼
┌──────────────────────────────────────────────────────────────────┐
│ This repository                                                  │
│  Markdown vault + graph.json, mirror-synced from a UC volume     │
└──────────────────────────────┬───────────────────────────────────┘
                               ▼
┌──────────────────────────────────────────────────────────────────┐
│ GitHub Actions → Quartz build → GitHub Pages                     │
│  → https://akhilesh-varma.github.io/databricks-digest-wiki/      │
└──────────────────────────────────────────────────────────────────┘
```

**Update cadence:** daily, 6 AM EST.

The pipeline source code lives in a separate, private repository — this public repo is the *output* artifact only, plus the workflow that builds the website from it.

---

## About the podcast

🎙️ **Daily Databricks Digest** is the audio companion to this wiki. Each weekday morning, a new ~10-minute episode covers the most important Databricks, lakehouse, and data-engineering news. The same automated pipeline that produces the audio also produces this repository — so the two stay perfectly in sync.

**How the wiki maps to the podcast:**

- Each `episodes/YYYY-MM-DD.md` page corresponds to **one podcast episode** of the same date
- Each `sources/YYYY-MM-DD/<rank>_<slug>.md` page is **one of the stories discussed in that episode's audio** (rank 1 = the top story / opening item)
- Listen to the audio while reading the wiki for the same content in two complementary forms: spoken narrative for context, written entries for reference and search

**Where to listen:**

- 🎵 **Podcast:** https://open.spotify.com/show/0o8UdVTvUVaNmcoxzgQ0zU
- 🔍 Or In Spotify podcast app — search **"Daily Databricks Digest"**

---

## Content disclaimer

> ⚠️ **Pages on this site are produced by an LLM extraction pipeline and may contain factual errors.**

- **Verify against the source.** Each story page includes a link to the original article — always check there before relying on a summary.
- **Entity extraction is automated.** Names of companies, technical concepts, and people are extracted from articles using an LLM and may be miscategorized or misattributed. Confidence scores are recorded in the page frontmatter.
- **Story summaries are derivative.** Summaries are paraphrased from publicly-available articles linked at each story page. Copyrights remain with the original publishers.
- **No affiliation.** This site is not affiliated with, endorsed by, or sponsored by Databricks Inc.

---

## Reporting errors or requesting takedowns

If your name or organization appears here and you'd like it corrected or removed, or if you spot a factual error in a summary:

👉 **[Open an issue](https://github.com/Akhilesh-Varma/databricks-digest-wiki/issues/new)**

Please include:

- The exact page URL (e.g. `/companies/your-company`) or file path in the repo
- A brief description of the error or the takedown reason
- (Optional) A link to documentation or context that supports the correction

 Acknowledgement of issue takes place within 7 days.

---

## License

- **Story summaries and extracted metadata** are derived from publicly-available articles. Underlying article copyrights remain with their original publishers.
- **The repository structure, automation workflow, and Quartz configuration files** in `.github/` are released under the [MIT License](LICENSE).

---

*This repository is generated and maintained by an automated pipeline. The README itself is hand-written and lives at `.github/README.md` so it survives the daily mirror sync.*
