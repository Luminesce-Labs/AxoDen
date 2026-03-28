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
  - axoden_zenodo_corpus.docx (definitive — Zenodo publication corpus)
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

## 4a. Zenodo Publication Corpus (Definitive Reference)

**Author:** Erkan Yalcinkaya · ORCID: 0009-0008-6435-3530
**Source:** `axoden_zenodo_corpus.docx` (March 2026)

17 DOI-registered publications across 10 research domains:

### Domain 1 — RF-AI Integration & Spectrum Assurance
| Publication | Date | Type | Zenodo |
|-------------|------|------|--------|
| AxoDen Spectrum Bridge (ASB) v4.0 | 2026-03-04 | Patent / Prior Art | 18863188 |

Four-gate admissibility sequence, physics-informed deterministic encoder, multi-scale wavelet tokenisation with ILFD phase encoding. Addresses NASEM Aug 2025 workshop RF-AI barriers.

### Domain 2 — Topological Certification & Evidence Graphs
| Publication | Date | Type | Zenodo |
|-------------|------|------|--------|
| Topology of Reasoning — Part I | 2026-02-25 | Preprint (Open) | 18769043 |
| Topology of Reasoning — Part II | 2026-03-04 | Preprint | 18862777 |
| Reflexive Epistemic Fabric | 2026-03-16 | Preprint | 19151991 |

Certification properties as topological invariants of evidence graphs. ER-topo.cert architecture. Topological Slack as continuous safety metric. Non-orientability as adversarial signal.

### Domain 3 — Mathematical Foundations & Information Physics
| Publication | Date | Type | Zenodo |
|-------------|------|------|--------|
| Information Physics for Safety-Critical AI | 2026-03-05 | Working Paper | 18876342 |
| AxoDen Unified Mathematical Backbone | 2026-02-13 | Preprint | 18633407 |
| Thermodynamics of Agency | 2026-01-04 | Preprint (Open) | 18146418 |
| Entropy-Frugal Intelligence (EFI) Conjecture | 2025-11-02 | Technical Note | 17506920 |
| Entropy-Bounded Data Pipelines & EFI | 2025-11-25 | Report | 17709557 |

Knuth's Information Physics applied to AI safety. Evidence graphs as posets with topological invariants as Knuthian valuations. Compositional safety envelopes. EFI Conjecture on entropy-budgeted cognition.

### Domain 4 — Safety Architecture (Core Kernel)
| Publication | Date | Type | Zenodo |
|-------------|------|------|--------|
| ASIL-M: Multi-Root Trust Architecture | 2025-11-23 | Report | 17690760 |
| Coprime-Factor Security Architecture | 2025-11-23 | Preprint | 17690358 |

Engineered independence as structural invariant (not assumed). Multi-root attestation, cryptographic heterogeneity, formal correlation elimination. IETF RATS draft filed.

### Domain 5 — Safety-Critical Failure Modes & Formal Proofs
| Publication | Date | Type | Zenodo |
|-------------|------|------|--------|
| Zombie Intent Hazard | 2026-02-25 | Preprint | 18768569 |

Previously undocumented safety vulnerability in write-ahead audit architectures. Session-bound verification formalised in TLA+. Gap not covered by IEC 61508 or DO-178C.

### Domain 6 — Cyber Defence & Ransomware Containment
| Publication | Date | Type | Zenodo |
|-------------|------|------|--------|
| AxoDen-K: Deterministic Cyber Defense | 2025-12-19 | Preprint | 17989744 |
| AxoDen-R: Deterministic Ransomware Prevention | 2025-12-20 | Preprint | 18000738 |
| Execution-Path Assurance for Ransomware | 2026-01-11 | Preprint (Open) | 18212915 |

Ransomware as bounded information-control problem. Deterministic state-space model. Confidence-gated, reversible-by-construction mitigations. Execution & Assurance Layer (EAL).

### Domain 7 — Critical Infrastructure & Cyber-Physical Systems
| Publication | Date | Type | Zenodo |
|-------------|------|------|--------|
| AxoDen Grid Flight Recorder — Micro-Grid Safety v2 | 2026-03-04 | Preprint | 18863456 |

Deterministic VSR control for microgrid actuation. Audit layer as active safety gate. Eliminates God Key Failure and Async Ingestion Failure. Aligned to NERC CIP, IEC 62351, IEC 61968/61970.

### Domain 8 — Quantum-Classical Safety Extensions
| Publication | Date | Type | Zenodo |
|-------------|------|------|--------|
| Compositional Framework for Hybrid Quantum-Classical AI Safety | 2026-01-11 | Preprint | 18213048 |
| Systems & Certification for Hybrid Quantum-Classical AI Safety | 2026-01-17 | Preprint | 18282922 |

Safety under partial observability. Admissible action control under bounded uncertainty. Extends Unified Mathematical Backbone to observability-limited regimes.

### Domain 9 — Multi-Agent Coordination
| Publication | Date | Type | Zenodo |
|-------------|------|------|--------|
| Cognitive Quad (C4): Formal Specification | 2025-11-22 | Model | 17680541 |
| Cognitive Quad — Applied Framework | 2025-11-22 | Model (Open) | 17680358 |

4D continuous cognitive profiling for multi-agent coordination. Stress-adaptive composition. Alignment, complementarity, and diversity metrics.

### Domain 10 — Essays & Foundational Thinking
| Publication | Date | Type | Zenodo |
|-------------|------|------|--------|
| In the Labyrinth of a Curious Mind | 2025-11-02 | Book (Open) | 17507073 |

Interdisciplinary essay collection on philosophy, science, technology, and culture.

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

Use these terms exactly as the corpus and site define them:

| Term | Meaning | Do NOT substitute |
|------|---------|-------------------|
| **Bounded trust** | Core positioning concept | "limited trust", "constrained trust" |
| **Kernel** | Core infrastructure layer | "engine", "core" |
| **Wedge** | Product vertical built on the Kernel | "module", "plugin" |
| **Spectrum Bridge** / **ASB** | RF-AI certification wedge | "RF module" |
| **Forensic Intelligence** | SOC investigation wedge | "forensics tool" |
| **Grid Flight Recorder** | Cyber-physical actuation wedge | "audit logger" |
| **Information physics** | Knuth's programme — foundational discipline | "information theory" alone |
| **Topological Slack** | Continuous safety metric from evidence graph topology | — |
| **ER-topo.cert** | Portable topological certificate format | — |
| **EFI Conjecture** | Entropy-Frugal Intelligence conjecture | — |
| **ASIL-M** | AI Safety Integrity Level — Multi-Root Trust | — |
| **Coprime-Factor Security** | Mathematically independent defence layers | — |
| **Zombie Intent Hazard** | Safety vulnerability in write-ahead audit architectures | — |
| **VSR** | Verification-Safety-Recovery control pattern | — |
| **Execution & Assurance Layer (EAL)** | Confidence-gated execution framework | — |
| **Cognitive Quad (C4)** | 4D multi-agent coordination framework | — |
| **Reflexive Epistemic Fabric** | Runtime graph of system assumptions/dependencies | — |
| **Unified Mathematical Backbone** | Compositional safety envelope framework | — |

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
