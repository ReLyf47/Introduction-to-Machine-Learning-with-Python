## Chapter 1 — Introduction

### Core Concepts

* Basics of Machine Learning
* Supervised vs. Unsupervised Learning
* Python Environment Setup

  * NumPy
  * SciPy
  * Matplotlib
  * Pandas
  * mglearn
  * Scikit-learn

### First Application

**Iris Species Classification** using **k-Nearest Neighbors (k-NN)**

---

## Chapter 2 — Supervised Learning

### Core Concepts

* Generalization
* Overfitting & Underfitting
* Classification vs. Regression

### Algorithms

| Category              | Algorithms                                                      |
| --------------------- | --------------------------------------------------------------- |
| **Instance-Based**    | k-Nearest Neighbors (k-NN)                                      |
| **Linear Models**     | Linear Regression, Ridge, Lasso                                 |
| **Classification**    | Logistic Regression                                             |
| **SVM**               | Linear SVM, Kernelized SVM                                      |
| **Probabilistic**     | Naive Bayes                                                     |
| **Trees & Ensembles** | Decision Trees, Random Forests, Gradient Boosted Decision Trees |
| **Neural Networks**   | MLP Classifier, MLP Regressor                                   |

### Model Uncertainty

* Decision Function
* `predict_proba`

---

## Chapter 3 — Unsupervised Learning & Preprocessing

### Preprocessing

* `StandardScaler`
* `MinMaxScaler`
* `RobustScaler`
* `Normalizer`

### Dimensionality Reduction & Feature Extraction

* Principal Component Analysis (**PCA**)
* Non-Negative Matrix Factorization (**NMF**)
* t-SNE

### Clustering

* k-Means
* Agglomerative Clustering
* DBSCAN

### Evaluation

* Adjusted Rand Index (**ARI**)
* Silhouette Score

---

## Chapter 4 — Data Representation & Feature Engineering

### Categorical Variables

* One-Hot Encoding
* Dummy Variables

### Feature Transformation

* Binning
* Discretization
* Polynomial Features
* Interaction Features

### Model & Feature Relationships

* Linear Models vs. Trees on Non-Linear Features
* Univariate Statistics
* Model-Based Feature Selection
* Iterative Feature Selection

---

## Chapter 5 — Model Evaluation & Improvement

### Cross-Validation

* Stratified k-Fold
* Leave-One-Out
* Shuffle-Split

### Hyperparameter Optimization

* Grid Search
* Randomized Search

### Classification Metrics

* Confusion Matrix
* Precision
* Recall
* F1-Score
* ROC-AUC

### Regression Metrics

* R²
* Mean Squared Error (**MSE**)

---

## Chapter 6 — Algorithm Chains & Pipelines

### Core Concepts

* Preventing Data Leakage
* Building Parameter Grids with `Pipeline`
* Feature Union
* Column Transformer

### Goal

Build reproducible machine learning workflows by combining preprocessing, feature engineering, and model training into a single pipeline.

---

## Chapter 7 — Working with Text Data

### Text Representation

* Bag-of-Words
* Tokenization
* Stop Words
* TF-IDF Rescaling
* N-Grams

### Advanced Text Processing

* Stemming
* Lemmatization

### Topic Modeling

* Latent Dirichlet Allocation (**LDA**)

---

## Chapter 8 — Wrapping Up

### Machine Learning Workflow

* Problem Definition
* Data Collection & Preparation
* Feature Engineering
* Model Selection
* Training
* Evaluation
* Deployment

### Production Machine Learning

* Framing Production Problems
* Testing
* Model Monitoring
* Maintaining Models

### Next Steps

* Deep Learning
* Advanced Machine Learning
* Production ML Systems

---

## Learning Path

```text
Introduction
     │
     ▼
Supervised Learning
     │
     ▼
Unsupervised Learning & Preprocessing
     │
     ▼
Feature Engineering
     │
     ▼
Model Evaluation & Improvement
     │
     ▼
Pipelines & Algorithm Chains
     │
     ▼
Text Data
     │
     ▼
Production & Deep Learning
```

> **Goal:** Build a solid foundation in machine learning, from fundamental concepts and classical algorithms to practical model evaluation, feature engineering, production workflows, and text processing.
