# GG_2025
This repository contains notebooks that reproduce the results of the preprint "Male _XIST_ expression in cardiac pseudo-glia does not induce X chromosome inactivation".

Notebooks and their contents:

* `1_assemble_datasets.ipynb`: create donor/cell type pseudobulks based on public heart single-cell RNA sequencing datasets.
* `2_split_by_xist.ipynb`: create donor/_XIST_ presence or absence pseudobulks based on glial/neuronal cells in heart datasets.
* `3_visualize_averages.ipynb`: load in pseudobulks and visualize the average expression of genes across datasets.
* `4_differential_expression.ipynb`: run DE tests on pseudobulks, regressing expression on sex, age, and pathology.
* `5_differential_expression_xistposneg.ipynb`: run (relatively computationally intensive) DE tests on _XIST_-positive/-negative pseudobulks, encoding donor ID as covariate.
* `6_differential_expression_xistposneg_viz.ipynb`: visualize results of DE tests.
* `7_arduini.ipynb`: inspect kallisto|bustools pseudoalignments of Arduini et al. rat heart data.
* `8_eraslan.ipynb`: inspect _XIST_ expression in male donors in Eraslan et al. data across a variety of tissues.
* `9_scBaseCount_mouse_scVI.ipynb`: cluster a variety of scBaseCount mouse datasets and check expression of _Xist_ globally and in pseudo-glia.
* `10_shen.ipynb`: cluster Shen et al. neonatal mouse heart and check expression of _Xist_.
* `11_qu.ipynb`: cluster Qu et al. realigned cynomolgus heart and check expression of _Xist_.

The pseudobulks, as well as the fit PyDESeq2 objects, can be found at https://zenodo.org/records/17111613.
