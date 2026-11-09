<div align="center">

# Christ Yvan (@Christ-yavn)
### **Open-Source Quantitative Microstructure, Formal DSL Compilers & Zero-Lookahead ONNX Inference**

[![ITC-SMC-EXTRACTOR CI](https://github.com/Christ-yavn/ITC-SMC-EXTRACTOR-/actions/workflows/ci.yml/badge.svg)](https://github.com/Christ-yavn/ITC-SMC-EXTRACTOR-/actions)
[![bot-quant CI](https://github.com/Christ-yavn/bot-quant-/actions/workflows/ci.yml/badge.svg)](https://github.com/Christ-yavn/bot-quant-/actions)
[![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)
[![Claude Code Workflow](https://img.shields.io/badge/Workflow-Claude_Code_(AGENT.md)-7C3AED)](https://github.com/Christ-yavn/ITC-SMC-EXTRACTOR-/blob/main/AGENT.md)

</div>

---

## 🔬 Open-Source Quantitative & AI Engineering Suite

I design and maintain open-source tooling focused on **eliminating look-ahead bias**, **formalizing discretionary market-microstructure concepts into deterministic Finite State Machines**, and **eliminating train-serve skew** between Python research pipelines and low-latency execution engines using **Claude Code** and **ONNX Runtime**.

| Repository | Release & License | CI Status | Core Technical Scope |
| :--- | :---: | :---: | :--- |
| **[ITC-SMC-EXTRACTOR-](https://github.com/Christ-yavn/ITC-SMC-EXTRACTOR-)** | 3.4.0 (MIT) | [![CI](https://github.com/Christ-yavn/ITC-SMC-EXTRACTOR-/actions/workflows/ci.yml/badge.svg)](https://github.com/Christ-yavn/ITC-SMC-EXTRACTOR-/actions) | **Formal DSL Compiler (SCRIBE-ICT v3/v4), Deterministic Dual-FSM Linter (ZONE_FSM × TRADE_FSM), & Native Claude Code Bridge (claude_agent_bridge.py)** compiling structural price-delivery primitives (FVG, BPR, Order Blocks, Liquidity Sweeps) into zero-lookahead Python 3.11+ & Pine Script v5/v6 engines with automated OHLC JSON test fixtures (33/33 unit tests). |
| **[ot-quant-](https://github.com/Christ-yavn/bot-quant-)** | 3.31.0 (MIT) | [![CI](https://github.com/Christ-yavn/bot-quant-/actions/workflows/ci.yml/badge.svg)](https://github.com/Christ-yavn/bot-quant-/actions) | **Zero-Lookahead Quantitative Research, Statistical Microstructure Forensics & Cross-Language ONNX Runtime Inference Framework** (Python 3.12 / ONNX / MQL5 C++) featuring causal shift=1 rolling windows, Poisson jump survival hazard models, live spread-adjusted EV gates, and a formal 18 KB [AGENT.md](https://github.com/Christ-yavn/bot-quant-/blob/main/AGENT.md) contract for Claude Code. |

---

## 🛠️ Primary Technical Stack

- **Languages**: Python 3.12, TypeScript 5+, MQL5 / C++, Pine Script v5/v6
- **Quantitative & ML Infrastructure**: ONNX Runtime, NumPy, Pandas, SciPy, Scikit-Learn, Causal Feature Engineering (shift=1), Deflated Sharpe Ratio & Out-of-Sample Grid Validation
- **Agentic Compilation & Verification**: Native Anthropic API & Claude Code CLI bridges (scripts/claude_agent_bridge.py), AGENT.md invariant contracts, deterministic static linters (lintFicheV3), and executable JSON OHLC test fixtures