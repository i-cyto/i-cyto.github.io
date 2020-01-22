# i-cyto.github.com

A companion github repository for [http://impact-cyto.inserm.fr](http://impact-cyto.inserm.fr)

All repositories at [https://github.com/i-cyto](https://github.com/i-cyto)

## News

**2020-02-07 [Atelier AFC 2020](https://afcytometrie.fr/jt-analyse-de-donnees-sophia-antipolis-fevrier-2020/)**
  - for installation see command lines below

**2019-09-17 [Atelier AFC 2019](posts/190917-atelier_afc_2019)**

**2019-09-13 [cytofkit](https://github.com/i-cyto/cytofkit)**
  - few updates to cytofkit, see [GUI screenshot](https://i-cyto.github.io/images/cytofkit_GUI_190913.png)
  - tested on a fresh install of R 3.6.1 (or 3.6.2) + Rtools 3.5 on **Windows** 10 or 7 64bits using the following commands to install packages
    - Please do copy/paste commands **line by line**
    - Whenever you get a message 'Update all/some/none? [a/s/n]:', answer **n**
    - If you get a dialog box asking to install from source, answer either **no**
```
if (!requireNamespace("BiocManager", quietly = TRUE)) install.packages("BiocManager")
BiocManager::install("flowCore")
BiocManager::install("uwot")
BiocManager::install("devtools")
devtools::install_github("i-cyto/cytofkit")
devtools::install_github("i-cyto/cytofast")
```

**2019-09-13 [cytofast](https://github.com/i-cyto/cytofast)**
  - import FCS from cytofkit
  - nice [heatmap](https://i-cyto.github.io/images/heatmap_cytofast.png) of combined markers and percentages

**2019-06-06 [cytofkit](https://github.com/i-cyto/cytofkit)**
  - Clustering parameters are clearly organized to each method in the GUI
  - Compensation is taken into account
  - Range for cluster is set to max + 1
