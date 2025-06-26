# Statistical-Bias-in-ML
A deeper dive on statistical bias within black-box models using interpretability tools and fairness metrics.

**Authors:** Eric Haslam, Jack Cook, Dr. Zachary M. Boyd, Dr. Alice C. Schwarze  
**Date:** June 2025  

---

## Overview  
This repository contains code and documentation for our study on interpretability and fairness in recidivism prediction using model-agnostic explanation methods (LIME, SP-LIME, SHAP) alongside fairness toolkits (IBM AIF360, Microsoft Fairlearn). We train an XGBoost classifier on the COMPAS “cox-violent-parsed” dataset, then explore:  
- **Feature attributions** at both **instance** (LIME, SHAP) and **population** levels (SP-LIME, SHAP plots).  
- **Fairness metrics** and **mitigations** (statistical parity, equalized odds) via AIF360 and Fairlearn.  
- **Tree visualizations** to inspect raw model structure.

---

## Getting Started

### Prerequisites  
- Python 3.8+  
- `xgboost`, `pandas`, `numpy`, `scikit-learn`  
- `matplotlib`, `graphviz`, `IPython`  
- IBM AIF360 (`aif360`), Fairlearn (`fairlearn`)  

