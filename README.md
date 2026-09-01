# GAIN Web Application Tools

A small set of self-contained, client-side HTML tools for SEO/outreach workflows. No backend, no build step — everything runs entirely in the browser (nothing is uploaded anywhere), so it's safe to host as a static site.

## Tools

| Tool | File | What it does |
|---|---|---|
| Home | `index.html` | Landing page linking to all tools |
| CSV Merger | `CSV_MERGE.html` | Merges multiple CSV files into one, optionally unioning headers |
| Keyword Generator | `KEYWORDS_GENERATOR.html` | Builds Google/Bing/DuckDuckGo search-operator query combinations (resource pages, guest posts, in-content, mentions-to-links) |
| Page Finder | `PAGE_FINDER.html` | Filters a list of URLs down to likely skyscraper/resource-page prospects |

The nav bar on each page also links to a **Domain Rate** tool hosted externally at `https://teamwonk.com/drtool/` — that one lives outside this repo.

## Using it (no setup required)

Once this repo is published with GitHub Pages (see below), just share the Pages URL — anyone on the team can open it in a browser and use the tools directly. Nothing needs to be installed.

## Publishing with GitHub Pages

1. Push this folder to a GitHub repository (see commands below).
2. In the repo on GitHub: **Settings → Pages**.
3. Under **Build and deployment → Source**, choose **Deploy from a branch**.
4. Branch: `main`, folder: `/ (root)` → **Save**.
5. GitHub will give you a URL like `https://<your-username>.github.io/<repo-name>/` within a minute or two. Share that link with the team.

## Running locally instead

No server needed — just open `index.html` directly in a browser (double-click it, or `open index.html` / `start index.html`).

## Repo structure

```
.
├── index.html
├── CSV_MERGE.html
├── KEYWORDS_GENERATOR.html
├── PAGE_FINDER.html
└── README.md
```

## Adding a new tool later

1. Add the new `.html` file to the repo root.
2. Add a card for it in `index.html` (`.tools-grid`) and a nav link (`.nav-links`) in every existing page for consistency.
3. Commit, push — GitHub Pages redeploys automatically within a minute or two.
