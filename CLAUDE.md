# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repo is

Static marketing site for **Luminesce Limited** (luminescelimited.com), served as plain files — no build step, no framework, no package manager. The repo directory is still named `AxoDen-Website` from before the rebrand; AxoDen is now the product line within Luminesce, not the company.

## Stack

- Plain HTML5 per page, one shared stylesheet (`shared.css`), one shared script (`script.js`, mobile menu only).
- Self-hosted woff2 fonts (Source Serif 4, Syne) — preloaded in each page's `<head>`.
- No tests, no linters, no CI config in repo.

## Running locally

Any static server from the repo root, e.g.:

```
python3 -m http.server 8000
```

Then open `http://localhost:8000/`. There is no dev/prod distinction.

## Things that are easy to miss

**Cache-busting via query string.** Every page links assets as `shared.css?v=7` and `script.js?v=1`. When you change `shared.css` or `script.js`, bump the `v=` on **every HTML file** (currently 7 pages), otherwise returning visitors get stale assets. Keep the version identical across pages.

**Sitemap and SEO are hand-maintained.** `sitemap.xml` lists each public page with an absolute `https://luminescelimited.com/...` URL and a `lastmod` date — update both when you add, remove, or meaningfully change a page. `robots.txt` disallows `/privacy.html`; new private/legal pages should be added there. Each HTML file has its own `<title>`, meta description, canonical, OG, and Twitter card tags — duplicate the pattern when creating a new page rather than inventing a new shape.

**Content source of truth.** `Luminesce_Website_Content.md` is the long-form copy document the HTML is rendered from. When copy changes are requested, update both the markdown and the HTML; treat the markdown as the canonical text.

**Pages and primary nav.** Public pages: `index.html`, `kernel.html` (AxoDen Kernel), `defence.html`, `forensic-intelligence.html`, `grid-flight-recorder.html`, `research.html`. Plus `privacy.html` (not in nav, not in sitemap). The header/footer nav block is duplicated in every page — when adding a page to nav, edit each HTML file.

**Mobile menu.** The hamburger toggle in `script.js` requires a `.hamburger` button with `aria-controls="mobile-menu"` and a `#mobile-menu` overlay containing the nav `<a>` elements. New pages must include both, or the script silently no-ops.

**Accessibility patterns already in place** — preserve them when editing: skip link (`.skip-link` → `#main`), focus-visible outlines (rules in `shared.css`), `aria-label`/`aria-expanded` on the hamburger, `aria-label` on `<nav>` elements. Don't strip these when refactoring markup.

**Design tokens** live as CSS custom properties at the top of `shared.css` (`--ink`, `--teal`, `--gold`, `--max`, etc.). Use the tokens instead of hardcoding colors or the 1160px max-width.

**Lighthouse artifacts are gitignored** (`lighthouse.html`, `lighthouse-*.html`, `*.lh.json`) — fine to generate locally without polluting commits.

## Global communication principles

The user's global `~/.claude/CLAUDE.md` applies: no overselling, no flattery, no embellishment, plain factual reports, minimal ceremony, no superlatives, no metrics without baselines.
