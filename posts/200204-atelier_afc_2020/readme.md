Atelier AFC 2020
================

The commands are glued in a R Markdown [script](JT_AFC_2020_cytofkitlab.Rmd). We propose a [RECAP](200207-JTAFC_Pipeline_Recap.pdf) of the classical pipelines. To redo the R session, please follow the [PRESENTATION](200207-JTAFC_Cytofkit_Cytofast_Analysis.pdf).

You can simplify the selecion of markers by using a [text file](ck_markers_main.txt) of the markers to analyze. Just type this file name into the marker selection field.

Then it's possible to continue the analysis with cytofast. Here is the [html](JT_AFC_2020_cytofkitlab.html) resulting from the data exported from cytofkit. You need to define sample groups in a [meta.csv file](meta.csv). Then you get nice heatmaps, compute t-test of percentages and Volcano plots.

## Installation commands

  - Please do copy/paste commands **line by line**
  - Whenever you get a message 'Update all/some/none? [a/s/n]:', answer **n**
  - If you get a dialog box asking to install from source, answer **no**
```
if (!requireNamespace("BiocManager", quietly = TRUE)) install.packages("BiocManager")
BiocManager::install("flowCore")
BiocManager::install("uwot")
BiocManager::install("cytofast")

# install devtools if not already done
if (!requireNamespace("devtools", quietly = TRUE)) install.packages("devtools")
# install Rphenograph if not already installed
if (!requireNamespace("Rphenograph", quietly = TRUE))
  devtools::install_github("i-cyto/Rphenograph")
# install cytofkitlab
devtools::install_github("i-cyto/cytofkitlab")
```

## Updates
  - v1 2020-02-05: [html result](JT_AFC_2020.html) from [script](JT_AFC_2020_cytofkitlab.Rmd)
  
