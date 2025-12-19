This repository contains Python notebooks used to compute, analyze, and visualize SHAP (SHapley Additive exPlanations) values for multi-output models applied to hematological biomarkers. The focus is on comparing linear and nonlinear models in terms of feature importance and interpretability across multiple related outputs.

For more details about the experiments, please read Section 3 (Simulation Experiments) in the paper: 

In particular, the analysis targets three clinically relevant hematological quantities:

-) HCT (%) — Hematocrit

-) HGB (g/dL) — Hemoglobin concentration

-) RBC (10¹²/L) — Red blood cell count

The repository includes scripts to:

1) train linear and nonlinear multi-output models,

2) compute SHAP values for each output,

3) aggregate Mean Absolute SHAP values,

4) generate bar plots and beeswarm plots,

5) and construct publication-ready composite figures.

The dataset consists of 30,000 synthetic samples designed to emulate a complete blood count (CBC)-like clinical dataset enriched with demographic, anthropometric, biochemical, and lifestyle-related variables.

Each sample corresponds to a single (synthetic) individual and includes:

-) Input features (predictors): demographic, clinical, biochemical, and lifestyle variables.

-) Target variables (responses): HCT, HGB, and RBC, treated jointly in a multi-output setting.

Each codes are written in a python script .ipynb. Each code can be launched directly (for example) by using Anaconda. Please, make sure to create a kernel compatible with pytorch, sklearn, numpy, etc.
