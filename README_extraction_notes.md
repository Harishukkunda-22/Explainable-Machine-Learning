# DSTDPT notebook output extraction

This package was prepared by extracting saved outputs from the uploaded `DSTDPT(4).ipynb` notebook.

## Contents
- `DSTDPT_Extracted_Notebook_Tables.xlsx`: HTML-rendered tables captured in the notebook outputs. The `Table_Index` sheet records the notebook cell and output location for each table.
- `Figures/`: PNG images embedded in saved notebook outputs.
- `Figure_Index.csv`: figure filenames and notebook cell provenance.
- `Table_Index.csv`: table provenance and dimensions.

## Important limitations
These are extracted saved notebook outputs, not a regenerated computational run.
Some tables in the notebook are previews (for example, `.head()` outputs) and contain only the displayed rows. They must not be represented as the complete 100-molecule source dataset unless independently checked against the original data files.
The notebook code references external runtime files under `/content` and `/content/DSTDPT_ML_Project`, including the clean 100-molecule ML dataset and xTB result files. Those external files are not embedded in the notebook itself. They therefore could not be reconstructed in full from this notebook file alone.
The figures are the images saved in the notebook outputs. They are not redrawn or altered.
Some tables may be repeated because the notebook contains repeated analysis or display cells. Their source cell locations are recorded in `Table_Index`.

## Reproducibility
To provide a fully reproducible public repository, also upload the original complete input dataset and any external CSV files required by the notebook, if available. Review all file paths and dependency installation instructions before asking reviewers to execute the notebook.
