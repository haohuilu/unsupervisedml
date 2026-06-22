# Unsupervised Machine Learning for Disease Prediction

Code and datasets accompanying the paper:

> **Lu, H., Uddin, S. (2024).** Unsupervised machine learning for disease prediction: a comparative performance analysis using multiple datasets. *Health and Technology*, **14**(1), 141–154. https://doi.org/10.1007/s12553-023-00805-8

## Overview

Most machine learning for disease risk prediction relies on **supervised** methods, but
labels are often missing — for example with undiagnosed or rare diseases. This study
compares **seven unsupervised (clustering) algorithms** across **15 health datasets**
(covering heart failure, diabetes, breast cancer, and more) using **six clustering
performance metrics**.

**Key finding:** No single model wins everywhere. DBSCAN performed best most often (31
times), followed by the Bayesian Gaussian Mixture (18) and Divisive/Agglomerative
clustering (15). Model and metric choice should be driven by the application.

### Algorithms compared
K-Means, MiniBatch K-Means, Agglomerative (Divisive) clustering, Affinity Propagation,
Spectral clustering, BIRCH, DBSCAN, Gaussian Mixture, and Bayesian Gaussian Mixture.

### Performance metrics
Adjusted Rand Index (ARI), Adjusted Mutual Information (AMI), Homogeneity, Completeness,
V-measure, and the Silhouette Coefficient.

## Repository structure

```
.
├── Unsupervised_Learning_for_disease_prediction.ipynb   # main analysis notebook
├── data/        # input datasets (one per analysis section, D1–D15)
├── results/     # clustering-metric tables produced by the notebook (D9r–D15r)
├── requirements.txt
└── README.md
```

See [data/README.md](data/README.md) for a description of each dataset.

## Getting started

```bash
# 1. (optional) create a virtual environment
python3 -m venv .venv && source .venv/bin/activate

# 2. install dependencies
pip install -r requirements.txt

# 3. launch the notebook from the repository root
jupyter notebook Unsupervised_Learning_for_disease_prediction.ipynb
```

Run the notebook **from the repository root** so the relative paths (`data/…`,
`results/…`) resolve correctly. Each section (D1–D15) loads one dataset, runs the
clustering algorithms, and writes a metrics table to `results/`.

> **Note:** Four input datasets used in the paper are public but not redistributed here
> (autism screening, prostate cancer, breast cancer Coimbra, and cervical-cancer risk
> factors). See [data/README.md](data/README.md) for details on which sections they
> correspond to.

## Citation

```bibtex
@article{lu2024unsupervised,
  title   = {Unsupervised machine learning for disease prediction:
             a comparative performance analysis using multiple datasets},
  author  = {Lu, Haohui and Uddin, Shahadat},
  journal = {Health and Technology},
  volume  = {14},
  number  = {1},
  pages   = {141--154},
  year    = {2024},
  doi     = {10.1007/s12553-023-00805-8},
  publisher = {Springer}
}
```

## License

Released under the [MIT License](LICENSE).
