
# Pre-Cascade Risk Screening in Interdependent Infrastructure Systems

**Supplementary materials for physics-informed cascade-risk prediction and mechanism-informed intervention prioritization.**

This repository provides supplementary materials accompanying a research study on prospective risk screening and mechanism-informed intervention prioritization in interdependent infrastructure systems. The proposed framework integrates physics-constrained cascade simulation, a relation-aware heterogeneous graph neural network (HGNN), and engineering motif analysis to anticipate severe cascading failures and characterize the structural and propagation patterns associated with cascade development.

The framework is evaluated on a synthetic Texas power–gas system using 7,800 simulated cascade trajectories spanning four disturbance families. By combining pre-cascade risk prediction with mechanism-specific analysis, the study provides an analytical basis for identifying locations that warrant further engineering assessment and evaluating candidate preventive interventions.

## 1. Research Overview

The study addresses two fundamental questions in cascading-risk management:

1. **Prospective risk screening:** Can severe cascading failures be anticipated using only disturbance information and infrastructure characteristics available before secondary failures emerge?
2. **Mechanism-informed prioritization:** Can recurrent structural configurations and failure-propagation patterns provide insights into where and how preventive interventions should be prioritized?

The proposed framework comprises three interconnected modules:

- **Module I — Physics-constrained cascade simulation:** Simulates infrastructure responses to spatial disturbances, capturing operational adjustments, component-state transitions, and cascading failure trajectories under physical and operational constraints.
- **Module II — Pre-cascade risk screening:** Employs a relation-aware HGNN to estimate severe-cascade probabilities using spatial disturbance information and pre-propagation infrastructure characteristics.
- **Module III — Mechanism-informed motif analysis:** Identifies recurrent structural configurations and failure-propagation patterns to characterize mechanism-specific infrastructure criticality and inform spatial intervention prioritization.

The HGNN achieved an average precision of **0.956** and an AUROC of **0.987** on previously unseen spatial disturbance fields. The calibrated predictions yielded a Brier score and expected calibration error of **0.047** each.

## 2. Repository Structure

```text
pre-cascade-risk-screening/
│
├── README.md
├── LICENSE
├── Motif definitions and identification.docx
│
└── Supplementary materials/
    │
    ├── Structural motifs_Figures/
    │
    ├── Propagation motifs_Figures/
    │
    ├── Structural_propagation_component level.png
    │
    └── moduleII_pre_cascade_HGNN_features_and_performance.xlsx
```

## 3. Supplementary Materials

The repository contains supplementary documentation, model-related results, and visualizations supporting the analyses presented in the accompanying manuscript.

| Material | Description |
|----------|-------------|
| [Motif definitions and identification.docx](Motif%20definitions%20and%20identification.docx) | Engineering motif definitions and identification criteria, including structural and propagation motifs. |
| [Structural motifs_Figures](Supplementary%20materials/Structural%20motifs_Figures/) | Supplementary visualizations of structural motifs associated with infrastructure susceptibility. |
| [Propagation motifs_Figures](Supplementary%20materials/Propagation%20motifs_Figures/) | Supplementary visualizations of propagation motifs identified from simulated cascade trajectories. |
| [Structural_propagation_component level.png](Supplementary%20materials/Structural_propagation_component%20level.png) | Component-level visualization integrating structural and propagation motif information. |
| [HGNN features and performance.xlsx](Supplementary%20materials/moduleII_pre_cascade_HGNN_features_and_performance.xlsx) | Supplementary information on HGNN input features and predictive performance. |

The supplementary workbook `moduleII_pre_cascade_HGNN_features_and_performance.xlsx` provides additional information related to the pre-cascade HGNN model, including its feature representation and predictive performance.

The HGNN estimates severe-cascade probabilities using information available before secondary failure propagation, enabling prospective risk screening under previously unseen spatial disturbance patterns.

These materials complement the model formulation, validation procedures, and performance evaluation reported in the manuscript.

## 4. Data Availability and Reproducibility

The supplementary materials provided in this repository support the interpretation and assessment of the methods and results presented in the accompanying study.

The repository currently includes supplementary documentation, figures, and an HGNN-related workbook. It does not constitute a complete release of the cascade simulation environment, trained HGNN model, source code, or full simulation trajectory dataset.

Additional data supporting the findings of this study are available from the corresponding author upon reasonable request.


## 5. License

This repository is distributed under the [MIT License](LICENSE).

The license applies subject to the terms specified in the LICENSE file. Third-party materials, where applicable, remain subject to their respective licenses and permissions.

