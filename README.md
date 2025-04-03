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

This repository follows a clear and organized folder structure to support a fully reproducible workflow:

assets/: Contains static assets such as images, schematics, .bib reference files, CSL citation styles, and other non-code files.

code/: Contains all scripts for data processing, cleaning, analysis, and visualization. Subfolders may be added for different stages of the analysis. You can access the full set of analysis scripts here.

data/: Contains raw and processed datasets used in the analysis. Subfolders are organized to separate raw data from cleaned/processed data.

products/: Contains project deliverables such as reports, manuscripts, slides, or supplementary materials. These are primarily created using Quarto.

products/manuscript/: Contains the project manuscript/report written in Quarto.

products/slides/: Contains slide decks or presentations related to the project.

results/: Contains all code-generated outputs such as tables, figures, .rds files, and processed result files. These are generated programmatically and should not be manually edited.

README.md: Provides an overview of the project structure, instructions, and reproducibility details (this file).

.Rproj file: Defines the RStudio project workspace.

Hidden files (e.g., .gitignore, .Rprofile): Used for R and GitHub configuration and can be ignored.




# Reproducibility Instructions
All required data files and scripts are included in this GitHub repository. To fully reproduce this project and its results, follow the steps below in the order listed:

1. processing_code.Rmd – Processes and cleans the raw data.
2. exploration.Rmd – Conducts exploratory data analysis.
3. analysis.Rmd – Performs statistical analysis on the processed data.
4. modeling.Rmd – Builds and evaluates statistical or machine learning models.
5. land_model.Rmd – Applies land model analysis (if applicable).
6. map_images.Rmd – Generates geographic visualizations and maps.
7. Manuscript.Rmd – Compiles the final manuscript report.
8. Supplement.Rmd – Compiles any supplementary materials.

Running these scripts in order will allow you to reproduce the full analysis workflow and outputs.




