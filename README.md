# THIS IS WORK IN PROGRESS*

# HiTOP_validation_submisison
This is a repo for code accompanying the manuscript "Test-Retest reliability and measurement invariance of a subset of the HiTOP internalizing scales with a two-week time window"

# Authors

[Marie Zelenina](https://github.com/mariezelenina)

Francisco Pereira

[Dylan M. Nielson](https://github.com/Shotgunosine)

# Important links

## Preregistration
- https://osf.io/xpa7v/

# Abstract

This is the repostory for the code used for the manuscript "Test-Retest reliability and measurement invariance of a subset of the HiTOP internalizing scales with a two-week time window". 
[TODO]

# How to run the code

All preprocessing and analyses were conducted in Python, using Jupyter Notebooks.

This directory has eight .ipynb files. Seven files with names starting with "notebook_analysis" are used for data analysis; one file with name starting with "notebook_graph" is used for plotting the data.

Notebooks should be ran cell by cell, paying attention to comments which cells to run for which dataset (general population or enriched population or combined) and which visit (initial or recontact).

- The notebook ***notebook_analysis_1_preprocessing_CLEAN.ipynb*** preprocesses raw datasets and saves the data in the format for future analysis.

- The notebook ***notebook_analysis_2_descriptive_both.ipynb*** outputs descriptive statistics (sex and age distribution) and can be used to plot visiual representations of these statistics.

- The notebook ***notebook_analysis_3_ICC_both.ipynb*** performs itracorrelation analyses (ICC).

  - The notebook ***notebook_graph_hitop_iccs.ipynb*** plots figure [TODO figure number from manuscript]: ICC for both datasets.

- The notebook ***notebook_analysis_4_cronbachs.ipynb*** calculates Cronbach's alpha.

- The notebook ***notebook_analysis_5_cfa_functions.ipynb*** assesses measurement invariance by performing confirmatory factor analyses (CFA) for HiTOP scales.

- The notebook ***notebook_analysis_6_cfa_baars_gad_phq.ipynb*** assesses measurement invariance by performing confirmatory factor analyses (CFA) for BAARS, GAD and PHQ scales.

- The notebook ***notebook_analysis_7_conv_div.ipynb*** performs convergent and divergent validity hypotheses.

# Where/how to get the data

TODO

# How to run the code

To run the analysis, open the desired .ipynb file.
Each main analysis file contains functions for loading files, preprocessing and analysis. 
Notebooks are to be run block by block.
Please submit an issue in this repository or reach out to [Marie Zelenina](https://github.com/mariezelenina) or [Dylan Nielson](https://github.com/Shotgunosine) with questions.

## How to install dependencies

We use the following python libraries: 

jupyter notebook pandas numpy matplotlib scikit-learn scipy itertools seaborn rpy2 pingouin statsmodels random

and the following R packages (for CFA analysis):

utils lavaan semtools stringr reticulate

You can create a conda environment with:
`conda env create -p ./env -f environment.yml`
