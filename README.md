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

This project follows a clear and organized folder structure:

assets/: Contains static files such as images, schematics, .bib reference files, CSL citation styles, or any non-code-based content.

code/: Contains all code for data processing, cleaning, analysis, and visualization. Subfolders may be added for different stages of the analysis.

data/: Stores the raw and processed datasets used in the analysis. Subfolders organize the data at different stages (e.g., raw, processed).

products/: Contains deliverables such as reports, manuscripts, slides, or supplementary files. These are mostly generated using Quarto.

manuscript/: Contains the project report template written in Quarto.

slides/: Contains any presentation materials related to the project.

results/: Includes all code-generated outputs such as tables, figures, .rds data files, and processed data outputs. Results here should be generated programmatically and not manually edited.

README.md: Provides an overview and instructions for the project structure (this file).

.Rproj: Project file to work within RStudio.

Other hidden files (e.g., .gitignore, .Rprofile) are used to manage R and GitHub settings.




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




