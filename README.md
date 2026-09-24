# Introduction to Machine Learning with Python

This repository provides an end-to-end, reproducible implementation of the concepts, algorithms, and workflows presented in ***Introduction to Machine Learning with Python*** by Andreas C. Müller & Sarah Guido (O'Reilly).

It contains refactored Jupyter Notebooks (`.ipynb`) covering all 8 chapters, complete with mathematical foundations, production-grade `scikit-learn` code pipelines, and theoretical summaries.

---

## 📂 Repository Structure

```text
.
├── 01_introduction.ipynb            # Scientific Python Stack & Iris Classification
├── 02_supervised_learning.ipynb     # Linear models, Decision Trees, Ensembles, SVMs, MLPs
├── 03_unsupervised_learning.ipynb   # Preprocessing, Scalers, PCA, t-SNE, Clustering
├── 04_data_representation.ipynb     # Categorical encoding, Binning, Polynomials, Selection
├── 05_model_evaluation.ipynb        # Cross-Validation, GridSearch, ROC-AUC, Metrics
├── 06_algorithm_pipelines.ipynb     # Leakage prevention, Scikit-Learn Pipelines
├── 07_text_data.ipynb               # Bag-of-Words, TF-IDF, N-Grams, Topic Modeling (NMF/LDA)
├── 08_wrapping_up.ipynb             # Baselines, End-to-End Production Pipelines, Error Auditing
├── requirements.txt                 # Fixed dependency environment specifications
└── README.md                        # Comprehensive repository documentation

```

---

## 📖 Chapter Index & Summary

| Chapter | Core Focus | Main Algorithms & Tools | Key Concepts / Deliverables |
| --- | --- | --- | --- |
| **[01. Introduction](https://www.google.com/search?q=01_introduction/01_introduction.ipynb&utm_source=gemini)** | Python Scientific Stack & First ML Application | `NumPy`, `SciPy` (CSR/COO), `Pandas`, `Matplotlib`, $k$-NN | Dense vs. sparse representations, hold-out $75/25$ splitting, pairwise scatter matrices. |
| **[02. Supervised Learning](https://www.google.com/search?q=02_supervised_learning/02_supervised_learning.ipynb&utm_source=gemini)** | Parametric, Non-Parametric & Ensemble Estimators | OLS, Ridge ($L_2$), Lasso ($L_1$), Logistic Regression, Trees, Random Forests, GBDT, RBF SVM, MLP | Bias-variance trade-off, model complexity, regularization strength ($C$ and $\alpha$), confidence metrics. |
| **[03. Unsupervised Learning](https://www.google.com/search?q=03_unsupervised_learning/03_unsupervised_learning.ipynb&utm_source=gemini)** | Scaling, Dimensionality Reduction & Clustering | `StandardScaler`, `MinMaxScaler`, PCA, t-SNE, $k$-Means, Agglomerative, DBSCAN | Data leakage prevention, 2D manifold projection, Adjusted Rand Index (ARI), Silhouette scores. |
| **[04. Feature Engineering](https://www.google.com/search?q=04_data_representation/04_data_representation.ipynb&utm_source=gemini)** | Categorical Encoding & Feature Selection | `ColumnTransformer`, `OneHotEncoder`, `KBinsDiscretizer`, `PolynomialFeatures`, RFE | Non-linear capacity expansion in linear models, univariate ANOVA, model-based selection. |
| **[05. Model Evaluation](https://www.google.com/search?q=05_model_evaluation/05_model_evaluation.ipynb&utm_source=gemini)** | Cross-Validation & Diagnostic Metrics | Stratified $k$-Fold, `GroupKFold`, `GridSearchCV`, Precision/Recall, ROC-AUC | Imbalanced class evaluation, $F_1$-score aggregation (micro, macro, weighted). |
| **[06. Algorithm Pipelines](https://www.google.com/search?q=06_algorithm_pipelines/06_algorithm_pipelines.ipynb&utm_source=gemini)** | Encapsulating Workflows without Leakage | `Pipeline`, `make_pipeline`, `GridSearchCV` over pipelines | Encapsulated feature scaling during cross-validation, dynamic model architecture swapping. |
| **[07. Text Data](https://www.google.com/search?q=07_text_data/07_text_data.ipynb&utm_source=gemini)** | Natural Language Processing & Topic Modeling | `CountVectorizer`, `TfidfVectorizer`, N-Grams, NMF, LDA | Bag-of-words encoding, inverse document frequency weighting, unsupervised semantic topic extraction. |
| **[08. Production Workflows](https://www.google.com/search?q=08_wrapping_up/08_wrapping_up.ipynb&utm_source=gemini)** | Baselines, Integration & Error Analysis | `DummyClassifier`, `DummyRegressor`, `HistGradientBoosting`, Diagnostic Plots | Sanity checking complex models, full heterogeneous pipeline deployment, residual/error auditing. |

---

## 🛠️ Environment Setup & Installation

### Prerequisites

* Python 3.10 or higher
* Virtual environment tool (`venv` or `conda`)

### Step-by-Step Installation

1. **Clone the repository:**
```bash
git clone https://github.com/YOUR_USERNAME/Introduction-to-Machine-Learning-with-Python.git
cd Introduction-to-Machine-Learning-with-Python

```


2. **Create and activate an isolated Python environment:**
```bash
# Linux / macOS
python3 -m venv venv
source venv/bin/activate

# Windows (PowerShell)
python -m venv venv
.\venv\Scripts\Activate.ps1

```


3. **Install dependencies:**
```bash
pip install --upgrade pip
pip install -r requirements.txt

```



---

## 🚀 Usage

Launch JupyterLab or Jupyter Notebook to run and explore the execution notebooks:

```bash
jupyter lab

```

### Running Individual Notebooks Programmatically

To execute a notebook non-interactively via CLI:

```bash
jupyter nbconvert --to notebook --execute 01_introduction/01_introduction.ipynb

```

---

## 💡 Core Machine Learning Principles Covered

1. **Strict Leakage Prevention**: Preprocessing operations (scaling, imputation, feature selection) are calculated exclusively on training partitions inside `scikit-learn` `Pipeline` objects.
2. **Metric Selection Alignment**: Evaluation metrics are matched directly to domain goals—preferring Precision-Recall curves and ROC-AUC over plain accuracy for imbalanced datasets.
3. **Architecture Optimization**: Hyperparameter tuning via `GridSearchCV` searches across both preprocessing choices (e.g., bin count, scaling type) and estimator algorithms simultaneously.
