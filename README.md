# Financial Data Analyses 📈💰📊

This repo contains **reproducible financial data research** and modeling experiments. The goal is to turn noisy market + fundamentals data into **clean features**, run **leakage-aware evaluation**, and ship **decision-ready artifacts** (plots, tables, compact writeups, and sometimes lightweight tooling).

If you’re coming from my profile README, this repo is the “finance counterpart” to my aerospace and environmental work: same emphasis on structure, evaluation discipline, and clear outputs.

---

## What this repo covers

You’ll generally find work in a few buckets:

- Cross-sectional and time-series feature engineering (prices, returns, vol, fundamentals)
- Factor and signal research (ranking, weighting, portfolio construction)
- Backtesting and evaluation that avoids common pitfalls (leakage, lookahead, survivorship)
- Research artifacts that are easy to review (clean notebooks, exported figures, short reports)

---

## Featured work (start here)

### 📈 Multi-signal equity research (flagship style)
A disciplined, end-to-end workflow for developing and validating signals with **explicit splits** and reproducibility baked in.

What to look for:
- Clear separation of **TRAIN → VALIDATION → LOCKED → HOLDOUT**
- Documentation of data assumptions (trading calendar, corporate actions, universe definition)
- Metrics beyond returns (turnover, drawdowns, exposure, stability)

### 🧪 Signal diagnostics and evaluation tooling
Small utilities and notebooks that make it easy to answer “is this signal real?”:
- IC / rank-IC analysis, decay, stability by regime
- Turnover, capacity proxies, transaction cost sensitivity
- Feature correlation and redundancy checks

### 🧱 Data cleaning + canonical datasets
Pipelines that standardize messy raw data into analysis-ready formats:
- Adjusted price handling (splits/dividends if applicable)
- Point-in-time joins (when using fundamentals/macro)
- Consistent identifiers and universe filters

Replace these sections with links once the folders/notebooks exist, or point them at your best notebook(s).

---

## Repo structure (typical)

`data/` holds lightweight samples or metadata (large raw data is not committed).
`notebooks/` contains research notebooks (numbered or named by topic).
`src/` contains reusable feature engineering / evaluation code.
`reports/` contains exported figures and short writeups (png/html/pdf).

---

## Reproducibility and methodology notes

This repo emphasizes:
- Deterministic evaluation splits and documented experiment design
- No peeking: features and labels built using information available *as of that date*
- Transparent baselines and ablations (what moves performance vs what’s noise)
- Robust metrics (risk-adjusted performance, drawdowns, turnover, stability)

Where relevant, results include sensitivity checks (transaction costs, rebalance frequency, universe changes).

---

## Tech stack

Core: `Python` `pandas` `numpy` `scikit-learn`
Finance: `statsmodels` (when useful), optional backtesting tooling
Viz: `matplotlib` `plotly`
Data: `SQL` (Postgres/SQLite), `duckdb` (fast local analytics)

---

## How to run

```bash
# example
conda env create -f environment.yml
conda activate finance

jupyter lab
