# Scikit-learn Learning Journey

A hands-on collection of Jupyter notebooks for learning machine learning with Python and [scikit-learn](https://scikit-learn.org/). The notebooks move from preparing data to supervised learning, unsupervised learning, ensemble methods, model evaluation, and hyperparameter tuning.

## Topics covered

- **Preprocessing:** train/test splitting, missing-value imputation, feature scaling, categorical encoding, and column transformations
- **Supervised learning:** linear regression, logistic regression, K-nearest neighbours, decision trees, and support vector machines
- **Unsupervised learning:** K-means clustering, DBSCAN, and principal component analysis (PCA)
- **Ensemble learning:** random forests, AdaBoost, gradient boosting, stacking, and XGBoost
- **Evaluation and tuning:** confusion matrices, classification reports, K-fold cross-validation, `GridSearchCV`, and `RandomizedSearchCV`

## Repository structure

```text
scikit_learn/
├── preprocessing/
├── supervised_learning/
├── unsupervised_learning/
├── ensemble_learning/
├── requirements.txt
└── README.md
```

### Preprocessing

| Notebook | Topic |
| --- | --- |
| `preprocessing/train_test_split.ipynb` | Splitting data into training and test sets |
| `preprocessing/simple_imputer.ipynb` | Handling missing values with `SimpleImputer` |
| `preprocessing/featurescaling.ipynb` | Standardization and min-max normalization |
| `preprocessing/onehotencoding.ipynb` | Encoding nominal categories with `OneHotEncoder` |
| `preprocessing/ordinalencoding.ipynb` | Encoding ordered categories with `OrdinalEncoder` |
| `preprocessing/columntransformer.ipynb` | Applying transformations to selected columns |

### Supervised learning

| Notebook | Topic |
| --- | --- |
| `supervised_learning/linear_regression.ipynb` | Multiple linear regression |
| `supervised_learning/logisticregression.ipynb` | Binary classification with logistic regression |
| `supervised_learning/logistic_multiclass.ipynb` | Multiclass logistic regression using the digits dataset |
| `supervised_learning/KNN.ipynb` | K-nearest-neighbours classification |
| `supervised_learning/decisiontree.ipynb` | Decision-tree classification and evaluation |
| `supervised_learning/supportvectormachine.ipynb` | Support vector machine classification and key hyperparameters |
| `supervised_learning/K-foldcrossvalidation.ipynb` | K-fold cross-validation and `cross_val_score` |
| `supervised_learning/GridSearchCV.ipynb` | Exhaustive SVM hyperparameter tuning |
| `supervised_learning/RandomSearchCV.ipynb` | Randomized SVM hyperparameter tuning |

### Unsupervised learning

| Notebook | Topic |
| --- | --- |
| `unsupervised_learning/Kmeans_clustering.ipynb` | K-means clustering and the elbow method |
| `unsupervised_learning/DBSCAN.ipynb` | Density-based clustering with DBSCAN |
| `unsupervised_learning/PCA.ipynb` | Feature reduction with principal component analysis |

### Ensemble learning

| Notebook | Topic |
| --- | --- |
| `ensemble_learning/RandomForest.ipynb` | Random-forest classification |
| `ensemble_learning/boosting.ipynb` | AdaBoost and gradient-boosting classification |
| `ensemble_learning/stacking.ipynb` | Combining estimators with a stacking classifier |
| `ensemble_learning/XGboost.ipynb` | Gradient-boosted trees with XGBoost |

## Datasets

- `supervised_learning/500hits.csv` is used in selected supervised-learning notebooks.
- `unsupervised_learning/income.csv` is used for K-means clustering.
- Several notebooks use built-in scikit-learn datasets or generated sample data. Some examples fetch Seaborn datasets when run.

## Getting started

### 1. Clone the repository

```bash
git clone <your-repository-url>
cd scikit_learn
```

### 2. Create and activate a virtual environment

```bash
python -m venv .venv
```

**Windows (PowerShell)**

```powershell
.venv\Scripts\Activate.ps1
```

**macOS/Linux**

```bash
source .venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Launch Jupyter

```bash
jupyter notebook
```

Open a notebook and run its cells from top to bottom. A few examples download datasets or use packages not listed in `requirements.txt`, so an internet connection and any notebook-specific dependencies may be needed.

## Notes

This is a learning repository focused on clear, small experiments rather than production-ready machine-learning pipelines. The folders can be explored independently; for the smoothest learning path, start with preprocessing and then continue through the remaining sections.
