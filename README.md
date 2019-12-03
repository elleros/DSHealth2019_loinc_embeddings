# LOINC Embeddings

This repository provides the Python code and the Word2Vec embeddings to reproduce the scatter plots in the [KDD 2019 DSHealth Workshop](https://dshealthkdd.github.io/dshealth-2019/) paper "Evaluation of Embeddings of Laboratory Test Codes for Patients at a Cancer Center": [arxiv.org/abs/1907.09600](https://arxiv.org/abs/1907.09600). The code can be used as a starting point for furtrher in depth exploration of the embeddings.

The embeddings have been trained via Word2Vec skip-gram with EHR data from the [City of Hope National Medical Center](https://www.cityofhope.org/homepage). See paper for details on the training.

## Citation
If you use the material in your work, please cite our paper. __BibTeX entry:__

```
@inproceedings{larossi2019evaluation,
  title={Evaluation of Embeddings of Laboratory Test Codes for Patients at a Cancer Center},
  author={Rossi, Lorenzo A and Shawber, Chad and Munu, Janet and Zachariah, Finly},
  booktitle={KDD Workshop on Applied Data Science for Healthcare (DSHealth)},
  year={2019}
}
```

## Contents
* tsne\_plot\_kdd_dshealth2019.ipynb Jupyter notebook to generate the t-SNE plot.
* Data/ folder containing the Word2Vec embeddings for the LOINC codes as well as other files used to produce the *t*-SNE plot

**Note** you need to downlload the official LOINC CSV Table from [loing.org](https://loinc.org). The table file is necessary to provide a taxonomy of the LOINC codes and hence the classes showed in different colors in the scatter plot.

### How to download the official Loinc Table CSV file
* Create an account on LOINC.org (it's free) and log in
* Click on 'Downloads' (menu at the top of the page)
* Click on 'LOINC Table'
* Click on 'LOINC Table File (CSV)'
* Review and check the review the Copyright and Terms of Use note
* Click on 'Download': a zip archive will be downloaded on your machine
* Extraxct the Loinc.csv from the zip archive


