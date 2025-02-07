# Introduction

This repository contains data and code to reproduce the paper *CAPI-detect: machine learning in capillaroscopy reveals new variables influencing diagnosis* https://doi.org/10.1093/rheumatology/keaf073

The excel file contains raw data for the study and formulas for processing it to calculate the capillaroscopies with patterns that reached consensus, etc.

Then, the patterns have been exported to `gold_patterns_with_metrics_only_consensus.csv` and processed to add capillarocopy metrics with Capillary.io analysis. This is the file that the code will load to train and test models.

# Installing

This notebook has been tested with Python 3.12

Create a conda env with: `conda create -n capi_detect python=3.12`

Then install packages:

```sh
pip install -r requirements.txt
jupyter labextension install @jupyter-widgets/jupyterlab-manager
```

# Running

```sh
jupyter lab
```

Execute the notebook and you should get the same results as in `capi_detect.pdf`
