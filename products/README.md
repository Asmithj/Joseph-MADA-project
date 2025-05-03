
This **manuscript** folder contains all of the files and subfolders needed to build and distribute the main paper:

- `Manuscript.qmd`  
  Quarto source file for the manuscript. Render to Word or PDF via  
  ```bash
  quarto render Manuscript.qmd --to docx






Manuscript.docx
The generated Word document output from the Quarto render command.

.RData
Saved R workspace containing all of the data objects and models created during the analysis.

.Rhistory
R console history log capturing all commands run during development.

Images/
Folder of figure files (PNG, PDF) referenced in the manuscript text.

supplement/
Subdirectory containing the Supplementary‐Material QMD, its outputs (Word/PDF), and any supporting data or code snippets.