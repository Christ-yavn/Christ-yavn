# Christ Yvan — L1 MIAGE Student (Côte d'Ivoire) & Open-Source AI Developer

[![Location: Côte d'Ivoire](https://img.shields.io/badge/Location-C%C3%B4te%20d'Ivoire-orange)](https://github.com/Christ-yavn)
[![Academic Track: L1 MIAGE](https://img.shields.io/badge/University-Licence%201%20MIAGE-blue)](https://github.com/Christ-yavn)
[![Anthropic Claude Ecosystem](https://img.shields.io/badge/Anthropic-Claude%20Code%20Ecosystem-D97757)](https://github.com/Christ-yavn/youtube-video-extractor)
[![CI Status: 100% Passing](https://img.shields.io/badge/GitHub%20Actions%20CI-100%25%20Passing-brightgreen)](https://github.com/Christ-yavn/youtube-video-extractor/actions)

> **EN**: First-year **MIAGE** undergraduate student (*Méthodes Informatiques Appliquées à la Gestion des Entreprises* — Computer Science & Applied Information Systems) in **Côte d'Ivoire**. I build open-source AI education tools, multi-agent scientific verification skills for **Anthropic's Claude Code**, and civic-tech platforms for sustainable infrastructure.
>
> **FR**: Étudiant en **Licence 1 MIAGE** (*Méthodes Informatiques Appliquées à la Gestion des Entreprises*) en **Côte d'Ivoire**. Je conçois des outils open-source d'extraction de connaissances par l'IA, des systèmes multi-agents d'analyse quantitative pour **Claude Code**, et des plateformes numériques à impact local.

---

## Flagship Open-Source Projects for the Claude Ecosystem

### 1. [`Christ-yavn/youtube-video-extractor`](https://github.com/Christ-yavn/youtube-video-extractor) — **YouTube Video Extractor v4.0**
*Universal YouTube Video & Channel Extractor to Structured Courses, Master Handbooks (`MASTER.md`), `.jsonl` AI Datasets & Executable Code*
- **Why I built it as a student**: For students and self-learners in Côte d'Ivoire and around the world, YouTube is the largest free university — yet hours of visual explanations on slides, whiteboards, and charts are hard to study, search, or turn into structured notes and code.
- **What it does**:
  1. Accepts **any YouTube video, playlist, or channel** across 4 universal profiles (*General Courses*, *Software & CS*, *STEM & Mathematics*, and *Market Microstructure*).
  2. Automatically slices long videos into **35-minute (`2100s`) windows** so multimodal AI never loses mid-lecture visual details.
  3. Generates **8-section pedagogical course sheets** anchored to exact `[MM:SS]` timestamps, consolidates multi-video playlists into **`MASTER_<CONCEPT>.md`** textbooks, and exports **`.jsonl` datasets**.
  4. Validates every rule (`[R-xx]`, `[P-xx]`, Dual Finite State Machines) with a **10-criteria deterministic linter (`lintFicheV3`, 38/38 passing unit tests)** and compiles them into Python, TypeScript, or Course Modules via our native **Claude Code Bridge (`scripts/claude_agent_bridge.py`)**.
  5. Includes **Empirical Benchmark Test #1**: A real-world stress test on 106 technical YouTube videos across 4 deduplicated playlists.

### 2. [`Christ-yavn/quant-pod`](https://github.com/Christ-yavn/quant-pod) — **Quant Pod v3.0 (`SKILL.md` & 10 Python Engines)**
*Autonomous Multi-Agent Quantitative Research Skill & Scientific Verification Suite for Claude Code*
- **What it does**: A plug-and-play multi-agent skill (`quant-pod/SKILL.md`, `agent-quant-pod/SKILL.md`) and **10 zero-dependency pure-Python scientific engines** that help daily Claude Code users design, backtest, and audit quantitative hypotheses without statistical hallucinations or lookahead bias:
  - **Cryptographic Research Ledger (`research_integrity.py`)**: Append-only SHA-256 Merkle hash chain preventing post-hoc data snooping.
  - **NIST SP 800-22 & 800-90B Forensics (`prng_forensics.py`)**: Randomness and min-entropy $H_\infty$ diagnostics.
  - **Causal Alpha Discovery & Blind Adversarial Auditing (`quant_discovery_engine.py`, `quant_validation_engine.py`)**: UCB1 Bandit + AST complexity regularization, Bull vs. Bear debate, and FWER multiple-testing validation (Deflated Sharpe Ratio $N_{\text{eff}}$, Hansen SPA, Romano-Wolf StepM, and PBO).

---

## Civic-Tech & Academic Projects (Côte d'Ivoire)

- **[`Christ-yavn/ecocycle-ci`](https://github.com/Christ-yavn/ecocycle-ci) & [`Christ-yavn/Ecoloop-ci-backend`](https://github.com/Christ-yavn/Ecoloop-ci-backend)**: Full-stack Circular Economy & Smart Waste Management Platform for Côte d'Ivoire (React / TypeScript / Tailwind frontend + Python REST API & Geospatial Waste Sorting backend).
- **[`Christ-yavn/bot-quant-`](https://github.com/Christ-yavn/bot-quant-)**: Cross-Language Zero-Lookahead Quantitative Research & ONNX Runtime Inference Framework (Python 3.12 / ONNX / MQL5 C++).
- **[`Christ-yavn/christ-streamlit`](https://github.com/Christ-yavn/christ-streamlit)**: Interactive Logic & Deduction Web Application built with Python & Streamlit.

---

## Technical Stack
- **Languages**: Python 3.11/3.12, TypeScript (Node 22 ESM, React 19, Vite 8), MQL5 / C++, SQL
- **AI & Verification**: Anthropic Claude Code (`SKILL.md` & Compiler Bridges), Multimodal Video Extraction, Deterministic Linters, SHA-256 Merkle Audit Trails, GitHub Actions CI
