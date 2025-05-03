
## Data Sources  
Raw input data for all scripts can be downloaded from ClinEpiDB (PROMO trial):  
- **PROMO_Data.csv** (ClinEpiDB DS_8786631aaf)  
  https://clinepidb.org/ce/app/workspace/analyses/DS_8786631aaf/new/download  

Place this CSV into `data/raw-data/` before running any of the processing scripts.

---

## Folder Structure  
All analysis code lives here and is organized by purpose:

1. **processing-code/**  
   R/Quarto scripts that import `data/raw-data/PROMO_Data.csv`, clean and recode variables, and save:
   - `data/clean/PROMO_Data_clean.csv`
   - `data/clean/PROMOTE_Codebook.xlsx`
   - `data/processed-data/processeddata.rds`

2. **eda-code/**  
   R/Quarto scripts that perform exploratory data analysis:
   - Summary tables (`results/edatables/`)
   - Diagnostic plots (`results/edafigures/`)

3. **analysis-code/**  
   R/Quarto scripts for statistical modeling and machine‐learning:
   - Main logistic‐regression models
   - Interaction and subgroup analyses
   - ML workflows (random forest, XGBoost, elastic net)
   - Outputs saved to `results/tables/` and `results/figures/`

---

## Script Guidelines  
- **Inputs & outputs**  
  Each script must document at the top:
  ```yaml
  # Inputs:
  #   - data/raw-data/PROMO_Data.csv
  # Outputs:
  #   - data/clean/PROMO_Data_clean.csv
  #   - results/figures/...
  #   - results/tables/...
  
---
  
  
# Dependencies
  - Load all required R packages (e.g. library(tidyverse), library(tidymodels)) at the start of each file.

Modularity
  - Keep each script focused on one task (cleaning, EDA, modeling).
  - Name scripts with a numeric prefix to indicate order (e.g. 01-clean-data.Rmd, 02-eda-summary.Rmd, 03-modeling.Rmd).

Execution order
  - Run scripts sequentially:
  - processing-code/01-clean-data.Rmd
  - processing-code/02-generate-codebook.Rmd
  - processing-code/03-save-processed-data.Rmd
  - eda-code/01-exploratory-plots.Rmd
  - eda-code/02-summary-tables.Rmd
  - analysis-code/01-main-models.Rmd
  - analysis-code/02-interaction-models.Rmd
  - analysis-code/03-ml-workflows.Rmd
  
  
  
  
  
# Best Practices
  - Version control: commit each script after successful runs.
  - Reproducibility: set a seed (set.seed(1234)) for any randomized procedures.
  - Documentation: comment liberally, especially around data transformations and model specifications.
  - Output verification: after each script, check that expected files appear under data/ or results/.



  
  
  
  
  
  
  
  
  
  
  
  
  
  
