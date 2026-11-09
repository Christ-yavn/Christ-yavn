# Christ Yvan — Open-Source AI Compiler & Scientific Systems Engineer

[![Anthropic Claude Code Ecosystem](https://img.shields.io/badge/Anthropic-Claude%20Code%20Ecosystem-D97757)](https://github.com/Christ-yavn)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![CI Status: Passing](https://img.shields.io/badge/GitHub%20Actions%20CI-100%25%20Passing-brightgreen)](https://github.com/Christ-yavn/ITC-SMC-EXTRACTOR-/actions)

I build **deterministic, open-source developer compilers and multi-agent scientific skills for Anthropic's Claude & Claude Code ecosystem** — bridging unstructured multimodal video curricula and rigorous, reproducible code & research.

---

## Flagship Open-Source Suite for the Claude Ecosystem

### 1. [`Christ-yavn/ITC-SMC-EXTRACTOR-`](https://github.com/Christ-yavn/ITC-SMC-EXTRACTOR-) — **OmniScribe v4.0: Universal Video-to-Course, Formal Specification & AI Dataset Compiler**
- **What it does for developers, educators & researchers**: Transforms **any YouTube channel, university lecture playlist, or technical video curriculum** (`UNIVERSAL_COURSE_COMPILER`, `SOFTWARE_AND_ALGORITHMS`, `STEM_AND_QUANT_SCIENCE`, `MARKET_MICROSTRUCTURE_ICT`) into:
  1. **8-Section University-Grade Course Handbooks** anchored to exact `[MM:SS]` video timestamps,
  2. **Chronologically Consolidated Master Bibles (`MASTER_<CONCEPT>.md`)** across multi-video playlists,
  3. **Deterministic Dual-FSM Formal Specifications** (`[P-xx]`, `[D-xx]`, `[R-xx]`, `[REJ-xx]`, + 3 JSON test fixtures) verified by a 10-criteria linter (`lintFicheV3`),
  4. **Multi-Turn SFT / RAG Fine-Tuning Datasets (`.jsonl`)**,
  5. **Production Python, TypeScript, and Course Modules** compiled directly via our native **Claude Code Bridge (`scripts/claude_agent_bridge.py`)**.
- **Empirical Benchmark Test #1 Included**: Ships with a real-world 106-video benchmark dataset (4 deduplicated playlists with automatic 35-minute temporal slicing) and 38/38 passing unit tests in GitHub Actions CI.

### 2. [`Christ-yavn/quant-pod`](https://github.com/Christ-yavn/quant-pod) — **Quant Pod v3.0: Multi-Agent Scientific Research Skill (`SKILL.md`) & 10 Pure-Python Verification Engines**
- **What it does for daily Claude Code users**: A plug-and-play multi-agent scientific research skill (`quant-pod/SKILL.md`, `agent-quant-pod/SKILL.md`) and 10 zero-Lookahead Python verification engines designed to stop LLM statistical hallucination and backtest overfitting:
  - **Cryptographic Research Ledger (`research_integrity.py`)**: Append-only SHA-256 Merkle hash chain + pre-registration before any out-of-sample holdout test.
  - **NIST SP 800-22 & 800-90B Forensics (`prng_forensics.py`)**: Monobit, block frequency, runs, spectral FFT, Maurer universal, and min-entropy $H_\infty$ diagnostics.
  - **Causal Discovery & Blind Adversarial Auditing (`quant_discovery_engine.py`, `quant_validation_engine.py`)**: UCB1 Bandit + AST complexity regularization (`AlphaAgent` KDD'25) + Deflated Sharpe Ratio ($N_{\text{eff}}$), Hansen SPA, Romano-Wolf StepM, and Probability of Backtest Overfitting (PBO).

---

## Technical Stack & Engineering Standards
- **Languages**: TypeScript (Node 22 ESM, React 19, Vite 8), Python 3.11/3.12 (Scientific Computing, NumPy/SciPy, AST Compilers)
- **Verification**: Deterministic AST/Regex Linters, Synthetic JSON Fixtures, SHA-256 Merkle Audit Trails, GitHub Actions CI
- **Design**: 2026 Dark OLED / Alabaster OKLCH Design Tokens, 3D Spatial Perspective UI, WCAG 2.2 AA Accessibility
