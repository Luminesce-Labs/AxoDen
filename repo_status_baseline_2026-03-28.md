---
repo_name: AxoDen
repo_root: /Users/erkanyalcinkaya/projects/AxoDen
branch: main
git_describe: AxD2-10-g7137b8e
latest_commit: 7137b8e — Refocus About page on AxoDen product architecture (2026-03-27)
preferred_runtime: static-html
preferred_entrypoints:
  - index.html
authoritative_docs:
  - repo_status_baseline_2026-03-28.md
  - .claude/settings.local.json
verification_commands:
  - command: "open index.html"
    expected: "Site loads in browser with all navigation working"
  - command: "git status"
    expected: "On branch main, working tree reflects current edits"
status_summary:
  phase: "Active development — static product site"
  next_gate: "Commit and deploy pending changes across 7 modified HTML files"
update_policy:
  safe_updates:
    - verification_snapshot_results
    - git_metadata
    - open_items
  protected_fields:
    - repo_identity_and_scope
    - authoritative_source_ordering
    - preferred_runtime_path
    - vocabulary_rules
---

# AxoDen — Repo Status Baseline

**Date:** 2026-03-28
**Repo:** https://github.com/Luminesce-Labs/AxoDen.git
**Branch:** main
**Latest commit:** `7137b8e` — Refocus About page on AxoDen product architecture (2026-03-27)

---

## 1. Repo Identity

AxoDen is the **static product website** for Luminesce Limited. It presents the AxoDen platform — "bounded trust for AI by maths and information physics" — targeting regulated industries, critical infrastructure, and high-stakes AI systems.

**Organisation:** Luminesce Limited (via Luminesce-Labs GitHub org)

---

## 2. Technology Stack

| Layer | Detail |
|-------|--------|
| Format | Static HTML — no build system, no framework |
| Styling | Inline `<style>` blocks per page (CSS custom properties) |
| Fonts | System stacks + `syne-latin-700-normal.woff2` (self-hosted) |
| Media | `.mov` video asset (Spectrum Bridge hero), `.png` favicon |
| Hosting | Cloudflare (evidenced by `cloudflare/workers-autoconfig` remote branch) |
| Repo | GitHub — `Luminesce-Labs/AxoDen` |

---

## 3. Site Structure

| File | Purpose |
|------|---------|
| `index.html` (49 KB) | Homepage — AxoDen overview, bounded trust positioning |
| `kernel.html` (51 KB) | AxoDen Kernel — bounded trust infrastructure for AI |
| `forensic-intelligence.html` (34 KB) | Forensic Intelligence — deterministic SOC investigation |
| `spectrum-bridge.html` (26 KB) | Spectrum Bridge — RF-AI certification layer |
| `grid-flight-recorder.html` (27 KB) | Grid Flight Recorder — verified actuation for cyber-physical systems |
| `research.html` (36 KB) | Research — 17 DOI-registered publications |
| `privacy.html` (15 KB) | Privacy notice |
| `about.html` | **Deleted** (removed in latest commit, content likely folded into other pages) |

**Static assets:**
- `favicon-32.png` — site favicon
- `syne-latin-700-normal.woff2` — Syne 700 webfont
- `AxoDen__The_Circuit_Breaker_for_AI_Reality - Small.mov` — hero video (~10.5 MB)

---

## 4. Product Architecture (as presented on site)

AxoDen consists of a **kernel** and product **wedges**:

- **Kernel** — core bounded trust infrastructure
- **Spectrum Bridge** — RF-AI certification layer
- **Forensic Intelligence** — deterministic SOC investigation
- **Grid Flight Recorder** — verified actuation for cyber-physical systems

---

## 5. Current Working State

**Modified files (uncommitted):**

| File | Status |
|------|--------|
| `about.html` | Deleted |
| `forensic-intelligence.html` | Modified |
| `grid-flight-recorder.html` | Modified |
| `index.html` | Modified |
| `kernel.html` | Modified |
| `privacy.html` | Modified |
| `research.html` | Modified |
| `spectrum-bridge.html` | Modified |

Seven HTML files have pending modifications. The `about.html` page has been removed.

---

## 6. Commit History (recent)

| Date | Hash | Message |
|------|------|---------|
| 2026-03-27 | `7137b8e` | Refocus About page on AxoDen product architecture |
| 2026-03-22 | `b2f6858` | Refine site messaging around bounded trust for AI |
| 2026-03-21 | `04412d2` | Replace Spectrum Bridge video with smaller MOV asset |
| 2026-03-21 | `732111a` | Add Spectrum Bridge hero video and MP4 asset |
| 2026-03-16 | `1531e6d` | Adjust AxoDen about heading |
| 2026-03-16 | `80a2d85` | Add ABOUT tab and update contract |
| 2026-03-14 | `c34260a` | Fix homepage footer script rendering |
| 2026-03-14 | `7b1f8b8` | Refocus site around kernel and two wedges |

Active development since 2026-03-10. ~15 commits total. Commit cadence: several per week.

---

## 7. Vocabulary Rules

Use these terms exactly as the site defines them:

| Term | Meaning |
|------|---------|
| **Bounded trust** | Core concept — not "limited trust" or "constrained trust" |
| **Kernel** | Core infrastructure layer — not "engine" or "core" |
| **Wedge** | Product vertical built on the Kernel |
| **Spectrum Bridge** | RF-AI certification wedge |
| **Forensic Intelligence** | SOC investigation wedge |
| **Grid Flight Recorder** | Cyber-physical actuation wedge |
| **Information physics** | Foundational discipline — not "information theory" alone |

---

## 8. Open Items

1. Seven modified HTML files are uncommitted — likely a coordinated messaging update
2. `about.html` deleted — verify no broken internal links remain
3. Large `.mov` file (10.5 MB) tracked in git — consider Git LFS if repo size becomes an issue

---

## 9. Verification Snapshot

```
Date: 2026-03-28
Branch: main
Commit: 7137b8e
Uncommitted changes: 7 modified, 1 deleted
Remote: origin → https://github.com/Luminesce-Labs/AxoDen.git
Remote branches: main, cloudflare/workers-autoconfig
```
