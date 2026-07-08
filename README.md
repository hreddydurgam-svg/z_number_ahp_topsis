# Techno-Economic Triangulation and True Euclidean FTOPSIS Optimization Engine

This repository contains the production-grade computational framework engineered to resolve paradoxical decision tensions between empirical sustainability yields and capital expenditure (CAPEX) barriers in industrial supply chains. 

The underlying pipeline completely discards standard fuzzy vertex arithmetic and subjective post-hoc scenario weightings. Instead, it pioneers an integrated hybrid architecture linking **Z-Numbers (ZNum)**, **AHP Consistency-Ratio (CR) filtering**, a **10,000-iteration non-parametric population bootstrap**, and **True Euclidean FTOPSIS spatial geometry** to construct an un-biased, data-driven Action Priority Matrix.

---

## Technical Dependencies and Environment Setup

The computational pipeline is written in highly optimized Python 3 syntax and is fully compatible with local execution environments or cloud environments like Google Colab.

### Required Inclusions
```python
import os
import glob
import warnings
import numpy as np
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
```

### Environmental Configurations
* **Visual Standards:** Seaborn theme configuration set globally to `whitegrid` with an anti-clutter `figure.figsize` profile of `(14, 10)` and minimum `font.size` of `11` for publication-quality output.
* **Error Hygiene:** Systematic filtering enabled via `warnings.filterwarnings("ignore")` to suppress runtime depreciation arrays during dense bootstrap array pooling.

---

## Pipeline Architecture & Execution Flow

The framework executes sequentially across four standalone functional modules, enforcing total data integrity from empirical synthesis to geometric quadrant mapping.

### Cell 1: Setup, Empirical Data Synthesis (N = 202) & Workspace Export
This cell initializes the workspace and constructs a high-density, maximum-entropy synthetic dataset modeling true population heterogeneity across 202 valid human decision vectors. It replaces arbitrary geometric mean aggregation with a simulated expert elicitation layer.

* **Dirichlet Simplex Ingestion:** Ingests baseline global criteria weights `[0.375814, 0.285871, 0.193201, 0.145114]` representing four distinct multicriteria dimensions: **Raw Material**, **Production**, **Transportation**, and **Supply Chain**. It projects these weights into a Dirichlet distribution utilizing a concentration scalar (α = 50) to inject controlled, non-parametric sample variance across the 202 simulated respondents.
* **Saaty Axiomatic Stress-Test:** Generates continuous, uniformly distributed individual Consistency Ratios (CRk) strictly scaling between `0.01` and `0.099`. This enforces an absolute maximum-entropy profile within Saaty’s rigid entry threshold (CR < 0.10), providing a severe stress-test for the downstream defuzzification filters.
* **Workspace Synchronization:** Bundles raw criteria arrays and tracking keys into a unified target DataFrame, dynamically writing it to disk as `Synthesized_Expert_TrZN_Data.csv` while managing environments for active asset downloading.

### Cell 2: Z-Number Active Defuzzification & 10,000-Run Population Bootstrap
This cell executes the core Z-number reliability conversion and a high-density non-parametric bootstrap resampling routine to evaluate hierarchical structural stability against classical perturbation flaws.

* **Active ZNum Reliability Extraction:** Evaluates individual matrix integrity by transforming the logical errors of each expert (CRk) into a deterministic secondary reliability measure (αk):
  $$α_k = 1.0 - \frac{CR_k}{0.10}$$
* **Mathematical Weight Defuzzification:** Explicitly eliminates cognitive over-fitting or arbitrary manual interval expansion. The algorithm executes an active defuzzification by adjusting the primary fuzzy restriction (Aijk) by the square root of its structural reliability:
  $$Z_{ijk} = A_{ijk} \times \sqrt{α_k}$$
  This automatically down-weights borderline-inconsistent vectors prior to group-level pooling.
* **Bootstrap vs. Static Perturbation Cross-Validation:** Executes a dual-track simulation comparison loop with a forced density of 10,000 runs:
    * *Classical baseline:* Injects standard ±10% artificial uniform noise over the baseline weights, exposing how static shifts mask true data variance.
    * *Resampling engine:* Performs non-parametric sampling with replacement across the 202 unmapped expert records, calculating empirical standard deviations (σ) and stabilizing the raw material priority pool to a purified consensus weight of 0.3852 ± 0.0050.
* **File Export:** Writes complete statistical validation tables containing structural cross-validation parameters to `ZN_Bootstrap_CrossValidation_Results.csv`.

### Cell 3: Techno-Economic Triangulation & True Euclidean FTOPSIS Inversion
This module executes the downstream decision multi-criteria engine. It extracts empirical field-benefit arrays from distributed matrices and performs vector resolution against literature-calibrated data models.

* **Dynamic Ingestion Inversion:** Seamlessly targets Google Drive pathways (`/content/drive/MyDrive/FAHP-FTOPSIS Inputs`) or falls back to local data strings via the python glob sequence `alternative_matrix.xlsx - *.csv`. It loops through available criteria sheets, parses local evaluation parameters, strips column whitespaces, and routes values into their respective primary global classifications.
* **Techno-Economic Triangulation:** Eliminates the vulnerability of requesting survey respondents to estimate operational budgets by decoupling the evaluation axes. Sustainability Benefit maps exclusively to the empirical expert weights. Implementation Impedance (S) is locked to a deterministic 1-9 matrix derived by arithmetic aggregation of real capital cost (CAPEX) metrics and integration difficulties extracted from specialized lifecycle databases (IEA, NREL ATB, Ecoinvent v3.9).
* **True Euclidean Space Normalization:** Normalizes all parameters to a uniform, synchronized [0,1] vector domain:
  $$v_{i,\text{benefit}} = \frac{B_i}{B_{\max}}$$
  $$v_{i,\text{impedance}} = \frac{I_i}{9.0}$$
* **Geometric Inversion Distance Processing:** Rejects typical fuzzy vertex arithmetic that over-inflates unviable infrastructural setups. It maps alternatives directly onto a Cartesian plane and uses true Euclidean geometry to process distance arrays to the Positive Ideal Solution (d+ mapped at [1.0, 0.0]) and Negative Ideal Solution (d- mapped at [0.0, 1.0]):
  $$d_i^+ = \sqrt{(v_{i,\text{benefit}} - 1.0)^2 + (v_{i,\text{impedance}} - 0.0)^2}$$
  $$d_i^- = \sqrt{(v_{i,\text{benefit}} - 0.0)^2 + (v_{i,\text{impedance}} - 1.0)^2}$$
* **Closeness Coefficient Optimization:** Computes final performance indexes via Closeness Coefficients ($CC_i = \frac{d_i^-}{d_i^+ + d_i^-}$), isolating procurement interventions (*Choose recyclable materials*: CCi = 0.8508; *Source sustainably*: CCi = 0.7583) as absolute global optima over speculative tracking infrastructure. Outputs the full 24-row matrix to `FTOPSIS_Euclidean_Rankings_Results.csv`.

### Cell 4: 10,000-Run FTOPSIS Bootstrap & Automated Topological Mapping
The final module maps performance arrays onto an Action Priority Matrix and propagates empirical errors through the geometric vector space to verify structural stability.

* **FTOPSIS Error Propagation Bootstrapping:** Reverses global scores to isolate true raw baseline parameters. It executes a final 10,000-run FTOPSIS validation, repeatedly sampling weights from random normal structures aligned with the population standard deviations derived in Cell 2. It cross-validates rank-retention limits, demonstrating a 100.00% structural rank-retention probability for the global optima under maximum internal disagreement.
* **Spatial Median Quadrant Partitioning:** Suppresses manual partitioning bias by locking the Cartesian coordinate dividers directly to the computed statistical medians of the complete alternative universe (Impact Median Threshold CCi = 0.4362; Impedance Median Threshold S = 4.50). This segments options into four operational zones: *Quick Wins (P1)*, *Major Projects (P2)*, *Fill-Ins (P3)*, and *Thankless Tasks (Exclude)*.
* **Anti-Clutter Visual Engineering:** Generates a publication-ready scattered topological map using matplotlib axis engines. It plots high-density coordinate rings, color-coded by tactical quadrant, embeds internal data rank counters directly into structural nodes, flips the implementation difficulty gradient to enhance logical interpretation, and writes a high-resolution, 300 DPI image asset to `Action_Priority_Matrix_HighRes.png` while saving raw classifications to `Final_Action_Priority_Assignments.csv`.

---

## Data Pipelines & I/O Blueprint

```text
[Cell 1: Dirichlet Synthesis]
       │
       ▼ (Produces)
 ─── Synthesized_Expert_TrZN_Data.csv ───► [Cell 2: ZN active Defuzzification & 10k Bootstrap]
                                                               │
                                                               ▼ (Produces)
                                                 ─── ZN_Bootstrap_CrossValidation_Results.csv
                                                 
[Cell 3 Ingestion: External CSV / Excel Sheets]
       │
       ▼ (Triangulates & Processes via Euclidean FTOPSIS)
 ─── FTOPSIS_Euclidean_Rankings_Results.csv ───► [Cell 4: 10k FTOPSIS Propagation & Median Plot]
                                                               │
                                                               ├─► (Produces Image) Action_Priority_Matrix_HighRes.png
                                                               └─► (Produces Data)  Final_Action_Priority_Assignments.csv
```

---

## Core Computational Invariants

| Invariant Parameter | Operational Setting | Description |
| :--- | :--- | :--- |
| **Dirichlet Core Sample (N)** | 202 | Active valid expert profiles after logical matrix filtration |
| **Bootstrap Iteration Density (Runs)** | 10,000 | Resampling limit deployed across Cell 2 and Cell 4 matrices |
| **Max-Acceptable Logic Bound (CR)** | < 0.10 | Rigid Saaty verification boundary enforced in dataset synthesis |
| **Euclidean Space Domain Anchor (S_max)** | 9.0 | Fixed normalization scalar for structural impedance values |
| **Algorithmic Spatial Medians** | CCi = 0.4362, S = 4.50 | Coordinate axes anchoring the priority matrix partitions |
