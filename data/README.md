# Datasets

Each section of the analysis notebook (`D1`–`D15`) uses one dataset. The table below maps
every notebook section to its input file, the disease it concerns, and its size. All
datasets are publicly available and were used here for non-commercial research.

| Section | Input file | Disease / topic | Rows | Features |
|---------|------------|-----------------|-----:|---------:|
| D1  | `D1.csv` | Heart disease (Cleveland) | 303 | 14 |
| D2  | `D2.csv` | Heart failure clinical records | 299 | 13 |
| D3  | `D3.csv` | Diabetes (Pima Indians) | 768 | 9 |
| D4  | `D4.csv` | Heart disease (Statlog) | 270 | 14 |
| D5  | `D5.csv` | Breast cancer (Wisconsin, mean features) | 569 | 6 |
| D6  | `D6.csv` | Cervical cancer behaviour risk | 72 | 20 |
| D7  | `D7.csv` | Liver disease (Indian Liver Patient) | 583 | 11 |
| D8  | `D8.csv` | Lung cancer | 309 | 16 |
| D9  | `thyroidDF(D9).csv` | Thyroid disease | 9,172 | 31 |
| D10 | `kidney_disease(D13).csv` | Chronic kidney disease | 400 | 26 |
| D11 | `indian_liver_patient(D14).csv` | Liver disease (Indian Liver Patient) | 583 | 11 |
| D12 | `Autism_Data(D18).arff` | Autism screening | — | — |
| D13 | `Prostate_Cancer(D17).csv` | Prostate cancer | — | — |
| D14 | `dataR2.csv` | Breast cancer (Coimbra) | — | — |
| D15 | `risk_factors_cervical_cancer(D22).csv` | Cervical cancer risk factors | — | — |

> The parenthetical labels in some filenames (e.g. `(D9)`, `(D13)`) refer to the original
> dataset identifiers from the authors' larger dataset pool and do **not** match the
> notebook section numbers. Use the **Section** column above as the source of truth.

## Not included here (D12–D15)

The four datasets above are public but are **not redistributed in this repository**. To
reproduce sections D12–D15, download the original datasets and place them in this `data/`
folder using the exact filenames the notebook expects:

- `Autism_Data(D18).arff` — Autism Screening Adult dataset
- `Prostate_Cancer(D17).csv` — Prostate cancer dataset
- `dataR2.csv` — Breast Cancer Coimbra dataset
- `risk_factors_cervical_cancer(D22).csv` — Cervical Cancer (risk factors) dataset

These are commonly available from the UCI Machine Learning Repository and Kaggle.

## Results

The clustering-metric tables produced by the notebook (`D9r.csv`–`D15r.csv`) live in the
[`../results`](../results) folder, not here. Each row is one algorithm and the columns are
the six performance metrics (ARI, AMI, Homogeneity, Completeness, V-measure, Silhouette).
