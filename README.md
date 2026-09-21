# Fairness Is Not Only an Endpoint

## Evaluating Pre-, In-, and Post-Processing Interventions in Contextual Bandits

This repository contains the code accompanying the manuscript:

**“Fairness Is Not Only an Endpoint: Evaluating Pre-, In-, and Post-Processing Interventions in Contextual Bandits.”**

The repository is provided for anonymous peer review and contains the code required to reproduce the principal experiments, statistical analyses, tables, and figures reported in the manuscript.

---

## Overview

The study investigates fairness interventions applied at three stages of a contextual multi-armed bandit pipeline:

1. **Pre-processing:** group–label reweighting of the replay distribution;
2. **In-processing:** demographic-parity-aware modification of the sequential action-selection rule;
3. **Post-processing:** group-specific decision thresholds estimated on a separate calibration set.

Three contextual-bandit policy families are evaluated:

- **LinUCB**
- **Linear Thompson Sampling (LinTS)**
- **EXP4**

Experiments are performed in:

- controlled synthetic contextual-bandit environments;
- the **Adult Income** dataset;
- the **COMPAS** dataset.

The main evaluation metrics include:

- average reward;
- demographic-parity gap;
- equalized-odds gap;
- true-positive-rate gap;
- false-positive-rate gap;
- UtilityGap;
- temporal fairness trajectories;
- Temporal DP Burden.

All principal experiments are repeated across **50 random seeds**.

## Repository structure

```text

.
├── README.md
├── requirements.txt
├── pyproject.toml
├── 01_synthetic_analysis.ipynb
├── 02_adult_analysis.ipynb
├── 03_compas_analysis.ipynb
└── src/
    └── fair_bandits/
        └── ...
```
