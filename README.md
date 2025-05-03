# Joseph-MADA Project – Spring 2025
 
# Overview
This repository contains the materials and analysis workflow for my primary data analysis project, completed as part of the Spring 2025 MADA course. The project is developed using R, Quarto, and GitHub, with an emphasis on clear organization, reproducibility, and transparency in data processing, analysis, and reporting.

# Introduction
This study investigates the relationship between malaria episode frequency and adverse birth outcomes among pregnant women in Uganda. Specifically, it assesses whether the type of Intermittent Preventive Treatment in pregnancy (IPTp) regimen, either sulfadoxine-pyrimethamine (SP) or dihydroartemisinin-piperaquine (DP) modifies this association. Additionally, the study examines whether higher gravidity reduces the risk of adverse birth outcomes among women under the age of 25.

# Pre-requisites
To run the analysis and reproduce the results in this repository, you will need the following tools and software:

R and RStudio
Quarto for dynamic reporting
Git and GitHub for version control
A reference manager that supports BibTeX (e.g., Zotero with Better BibTeX extension)
A word processor (e.g., MS Word or LibreOffice)
Optional: A TeX distribution (e.g., TinyTeX) if you wish to render PDF outputs.







# Template structure and content

1. data/
- raw-data/: Original PROMO trial CSV files
- clean/: Cleaned CSV plus codebook (XLSX)
- processed-data/: Final analysis dataset (.rds)


2. code/
- processing-code/: Data‐cleaning RMarkdown scripts
- eda-code/: Exploratory data analysis RMarkdowns
- analysis-code/: Modeling & statistical analysis RMarkdowns


3. results/
- figures/: Output figures (PNG/PDF)
- tables/: Output tables (.rds or image files)
- output/: Rendered reports (HTML/PDF)


4. products/
- manuscript/: Quarto source and compiled manuscript
- supplement/: Quarto source and compiled supplementary material


5. Images/
- Static images referenced in the manuscript


6. Manuscript.qmd
- Quarto source file for the main report


7. Manuscript.docx
- Generated Word document of the manuscript


8. .RData
- Snapshot of the R workspace (all objects)


9. .Rhistory
- R console history log of commands run


10. README.md
- Project overview and instructions


11. gitignore, .Rprofile
-  Git and RStudio configuration files



# Reproduction Requirements

To recreate this analysis from start to finish, you will need:
- R (version4.0 or later) with the rmarkdown ecosystem (and optionally bookdown for extended reporting).
- Git and a GitHub account for version control and collaboration.
- A BibTeX‑capable reference manager (e.g., Zotero, Mendeley) to handle citations.
-A Word‑compatible editor (such as Microsoft Word or LibreOffice Writer) for viewing or editing the final manuscript.

- (Optional but helpful) A spreadsheet application (e.g., Excel, LibreOffice Calc) to inspect the codebook and other data‐dictionary files.




# Data Sources
PROMO Trial Data
Retrieved from ClinEpiDB (Dataset ID DS_8786631aaf). Download the cleaned trial CSV here:
https://clinepidb.org/ce/app/workspace/analyses/DS_8786631aaf/new/download





# Reproducibility Instructions
To regenerate every output from scratch, run these Quarto/RMarkdown files in order:
- code/processing-code/01_clean_data.Rmd
- code/processing-code/02_generate_codebook.Rmd
- code/processing-code/03_save_processed_data.Rmd
- code/eda-code/01_exploratory_plots.Rmd
- code/eda-code/02_summary_tables.Rmd
- code/analysis-code/01_main_models.Rmd
- code/analysis-code/02_interaction_models.Rmd
- code/analysis-code/03_subgroup_models.Rmd
- products/manuscript/Manuscript.qmd
- products/supplement/Supplementary‑Material.qmd

Each script will produce the data, figures, tables, and final reports in results/ and products/. Follow this sequence to reproduce the full analysis and manuscript.


