# Data Mining Classification & Clustering

This project applies core data mining techniques across multiple datasets. It includes four supervised classification tasks and two unsupervised clustering tasks, with a focus on preprocessing, model comparison, and evaluation.

## Project Overview

The project is divided into two parts:

1. **Classification**: comparing Decision Tree, K-Nearest Neighbors, and Naive Bayes across four datasets.
2. **Clustering**: applying K-Means clustering and using inertia values with the elbow method to evaluate cluster quality.

## Datasets

| Task | Dataset Description | Rows | Columns | Target / Excluded Column |
|---|---:|---:|---:|---|
| Classification 1 | Student performance | 484 | 3 | `Pass` |
| Classification 2 | Purchase prediction | 380 | 4 | `Purchased` |
| Classification 3 | Mobile price classification | 2,000 | 21 | `price_range` |
| Classification 4 | Diabetes prediction | 764 | 9 | `Outcome` |
| Clustering 1 | Insurance/customer profile data | 1,337 | 10 | `charges` excluded |
| Clustering 2 | Vehicle emissions data | 18,967 | 114 | `emissions` excluded |

## Methods Used

### Classification Models

- Decision Tree Classifier
- K-Nearest Neighbors
- Naive Bayes

### Clustering Method

- K-Means Clustering
- Elbow method using inertia values

## Evaluation Metrics

For classification tasks, the models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

For clustering tasks, inertia values were compared for different values of `k`.

## Key Results

| Dataset | Best Model | Accuracy | F1-Score |
|---|---|---:|---:|
| Classification 1 | Naive Bayes | 0.8144 | 0.8142 |
| Classification 2 | KNN | 0.9079 | 0.9088 |
| Classification 3 | Decision Tree | 0.8425 | 0.8429 |
| Classification 4 | Naive Bayes | 0.6928 | 0.6921 |

For the clustering tasks, the first clustering dataset showed a clearer elbow pattern around `k = 4`, while the second clustering dataset showed weaker separation between clusters.

## Tech Stack

- Python
- Pandas
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## Project Files

- `notebooks/` — Jupyter notebooks for classification and clustering experiments.
- `data/` — CSV datasets used in the analysis.
- `docs/data_mining_project_report.pdf` — Final report summarizing methodology and results.
- `requirements.txt` — Python libraries required to run the notebooks.

## What I Learned

Through this project, I practiced applying supervised and unsupervised machine learning techniques, comparing model behavior across different datasets, using evaluation metrics, and interpreting results in a structured data mining report.
