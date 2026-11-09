# Hi, I'm Christ Yvan (`@Christ-yavn`)

### L1 MIAGE Student (Côte d'Ivoire) • Open-Source AI & Software Engineer

[![Location: Côte d'Ivoire](https://img.shields.io/badge/Location-C%C3%B4te%20d'Ivoire-orange)](https://github.com/Christ-yavn)
[![University: Licence 1 MIAGE](https://img.shields.io/badge/Academic%20Track-Licence%201%20MIAGE-blue)](https://github.com/Christ-yavn)
[![Claude Code Ecosystem](https://img.shields.io/badge/Anthropic-Claude%20Code%20Open%20Source-D97757)](https://github.com/Christ-yavn/youtube-video-extractor)
[![CI Status: Passing](https://img.shields.io/badge/GitHub%20Actions%20CI-100%25%20Passing-brightgreen)](https://github.com/Christ-yavn/youtube-video-extractor/actions)

---

## About Me

I am a first-year undergraduate student in **MIAGE (*Licence 1 — Méthodes Informatiques Appliquées à la Gestion des Entreprises*, Computer Science & Applied Information Systems)** in **Côte d'Ivoire**.

For students and self-taught developers in West Africa and around the world, two things make all the difference:
1. **Turning unstructured online videos into structured, verifiable knowledge**: YouTube is the world's largest free university, yet thousands of hours of lectures in computer science, mathematics, and quantitative engineering are locked inside long video streams without textbooks, formal definitions, or testable code.
2. **Preventing AI hallucinations in technical & scientific work**: When developers use AI coding assistants to turn lectures or research papers into software and quantitative models, they need deterministic linters and statistical verification tools so the code they build actually works in reality.

That is why I design and maintain open-source tools built specifically around **Anthropic's Claude and Claude Code**.

---

## Flagship Open-Source Projects

### 1. [`Christ-yavn/youtube-video-extractor`](https://github.com/Christ-yavn/youtube-video-extractor) — **YouTube Video Extractor (`v4.0.0`)**
*Universal Video-to-Course, Formal Specification, `.jsonl` AI Dataset & Code Compiler (`MIT License`)*

Instead of generating short, vague transcript summaries, **YouTube Video Extractor** is a full-stack application (React 19, TypeScript, Express, Python CLI) that turns **any educational YouTube video, university playlist, or technical channel** into structured study material and working software:

- **Works Across 4 Universal Domains (`src/utils/domainProfiles.ts`)**:
  1. `UNIVERSAL_COURSE_COMPILER`: University courses (MIAGE, CS, Business), MOOCs, and general tutorials.
  2. `SOFTWARE_AND_ALGORITHMS`: Programming tutorials, distributed systems, and AI engineering talks.
  3. `STEM_AND_QUANT_SCIENCE`: Mathematics, probability, physics, and econometrics lectures.
  4. `MARKET_MICROSTRUCTURE_ICT`: Financial market microstructure and algorithmic trading lectures.
- **How It Works Step by Step**:
  - **Automatic 35-Minute Slicing (`calculateSlices`)**: Long lectures (`> 35 minutes`) are automatically segmented into sequential 35-minute windows so multimodal extraction never loses detail in the middle of a 2-hour video.
  - **Dual-Layer Output (Human Course + Machine Spec)**: Every video produces **Part A** (an **8-section study handbook** with visual explanations anchored to exact `[MM:SS]` timestamps, worked examples, checklists, and flashcards) and **Part B** (formal parameters `[P-xx]`, boolean rules `[R-xx]`, Dual Finite State Machines, and 3 executable JSON test cases).
  - **10-Criteria Deterministic Linter (`lintFicheV3`, 38/38 Unit Tests)**: Automatically rejects vague placeholders (`TODO`, `TBD`), checks timestamp bounds against real video duration, and triggers surgical auto-repair before any sheet is validated.
  - **Cross-Video Consolidation & `.jsonl` Export**: Merges dozens of videos from the same channel into cohesive **`MASTER_<CONCEPT>.md`** textbook chapters and exports verified **`.jsonl` datasets** for RAG and LLM fine-tuning.
  - **Native Claude Code Compiler Bridge (`scripts/claude_agent_bridge.py` & Web UI)**: Connects directly to Anthropic's Claude (`ANTHROPIC_API_KEY` or `claude -p` CLI) to compile validated specifications into **6 targets**: University Course Handbooks, `.jsonl` Datasets, TypeScript modules, Python 3.11+ engines, PineScript v5/v6, and Red-Team Audits.
  - **100% Local Mode + Bring Your Own Keys (BYOK) + Benchmark Test #1**: Runs out of the box on any computer with zero cloud setup required, includes a local key vault for `GEMINI_API_KEY`, `ANTHROPIC_API_KEY`, and personal Google Drive OAuth, and ships with **Benchmark Test #1** (a real-world stress test on 106 technical videos, with the `10/10` reference specification `dg2-OsUXN60` preloaded for 1-click testing).

---

### 2. [`Christ-yavn/quant-pod`](https://github.com/Christ-yavn/quant-pod) — **Quant Pod (`v3.0.0`)**
*Autonomous Multi-Agent Quantitative Research Skill (`SKILL.md`) & 10 Pure-Python Scientific Verification Engines for Claude Code (`MIT License`)*

When a developer or student extracts a quantitative lecture or algorithm (for instance using `youtube-video-extractor`) and asks an AI agent to backtest it, most backtests fail in real life due to *p-hacking* (testing 100 variations and keeping the lucky winner), *look-ahead bias* (accidentally peeking at future data), or ignoring real transaction costs.

**`quant-pod`** solves this for daily **Claude Code** users through two components:
1. **A 2-Level Multi-Agent Skill (`quant-pod/SKILL.md`, `agent-quant-pod/SKILL.md`)**: Separates **Hypothesis Investigation**, **Causal Coding**, and **Blind Validation** across distinct subagents so the agent writing a strategy never grades its own work.
2. **10 Self-Tested Pure-Python Scientific Engines (`quant-pod/scripts/`, `numpy` & `scipy` only)**:
   - **`research_integrity.py`**: Append-only SHA-256 `HashChainLedger` that records every single trial (winners and losers) and seals 20% of the data in a cryptographic holdout so trial deletion is impossible.
   - **`event_backtester.py`**: Realistic bar-by-bar execution engine with live bid/ask spreads, post-jump slippage (`SL_GAP`), and `lookahead_truncation_test()` to catch any signal that changes when future bars are removed.
   - **`quant_discovery_engine.py`**: Checks formula originality using Abstract Syntax Trees (`ast_originality_penalty`), runs a pre-backtest Bull vs. Bear debate, and schedules experiments via a UCB1 bandit (`UCBFamilyBandit`).
   - **`quant_inference_engine.py`, `quant_validation_engine.py`, & `null_models.py`**: Runs Hansen's SPA, Romano-Wolf StepM, Deflated Sharpe Ratio on effective independent trials ($N_{\text{eff}}$), Probability of Backtest Overfitting (PBO), $2\times$ transaction cost stress tests, and $M \ge 100$ synthetic zero-edge null simulations.
   - **`prng_forensics.py`, `crypto_defi_engine.py`, `quant_scientific_arsenal.py`, & `deriv_quant_engine.py`**: NIST SP 800-22/90B randomness forensics, Uniswap v3 Loss-Versus-Rebalancing (LVR) & perpetual futures carry models, Marchenko-Pastur RMT + Hierarchical Risk Parity (HRP) portfolio sizing, and continuous-time Wonham Bayesian regime filters.

---

## Civic-Tech & Applied Software Projects

- **[`Christ-yavn/ecocycle-ci`](https://github.com/Christ-yavn/ecocycle-ci) & [`Christ-yavn/Ecoloop-ci-backend`](https://github.com/Christ-yavn/Ecoloop-ci-backend)**: Full-stack Circular Economy & Smart Waste Collection Platform built for communities in **Côte d'Ivoire** (React / TypeScript / Tailwind frontend + Python REST API & geospatial sorting backend).
- **[`Christ-yavn/bot-quant-`](https://github.com/Christ-yavn/bot-quant-)**: Real-world empirical case study applying `quant-pod` to audit 1.68 million ticks, refute an overfitted ML model, and run a strictly causal Python / ONNX / MQL5 C++ execution pipeline.
- **[`Christ-yavn/christ-streamlit`](https://github.com/Christ-yavn/christ-streamlit)**: Interactive Logic & Deduction Web Application built with Python and Streamlit.

---

## Présentation en Français

Bonjour ! Je m'appelle **Christ Yvan**, je suis étudiant en **Licence 1 MIAGE** (*Méthodes Informatiques Appliquées à la Gestion des Entreprises*) en **Côte d'Ivoire** et développeur open-source.

Je construis des outils open-source pour l'écosystème **Anthropic Claude & Claude Code** afin de :
1. **Transformer n'importe quelle vidéo ou chaîne YouTube éducative en cours structurés, datasets `.jsonl` et code exécutable** grâce à [**`youtube-video-extractor` (`v4.0.0`)**](https://github.com/Christ-yavn/youtube-video-extractor) (découpage temporel par tranches de 35 minutes, cours complet en 8 sections + spécification formelle, linter déterministe à 10 critères avec 38/38 tests unitaires, consolidation en manuels `MASTER_<CONCEPT>.md`, pont de compilation Claude Code vers 6 formats, et premier test grandeur nature sur 106 vidéos techniques).
2. **Garantir la rigueur mathématique et statistique des recherches générées par IA** grâce à [**`quant-pod` (`v3.0.0`)**](https://github.com/Christ-yavn/quant-pod), un skill multi-agents (`SKILL.md`) accompagné de 10 moteurs scientifiques en Python pur (`numpy`/`scipy`) intégrant une chaîne de hachage SHA-256 anti-triche (`HashChainLedger`), une sonde anti-lookahead par troncation et des tests économétriques de niveau institutionnel (Hansen SPA, Romano-Wolf StepM, DSR $N_{\text{eff}}$, PBO).

---

## Technical Stack & Contact

- **Languages**: Python (3.10–3.12, NumPy, SciPy), TypeScript / JavaScript (Node.js 22 ESM, React 19, Express, Vite 8), MQL5 / C++, SQL
- **AI & Verification**: Anthropic Claude API & Claude Code (`SKILL.md` & Compiler Bridges), Google Gemini Multimodal API, Deterministic Linters, SHA-256 Cryptographic Audit Ledgers, GitHub Actions CI
- **Email**: `yaochristyvan8@gmail.com`
