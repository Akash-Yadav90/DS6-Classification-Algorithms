# DS6-Classification-Algorithms
Comparison of Decision Tree, Random Forest, and SVM using scikit learn
# DS-6: Classification Algorithms Comparison

## 📌 Project Overview

This project compares three machine learning classification algorithms:

1. Decision Tree
2. Random Forest
3. Support Vector Machine (SVM)

The objective is to evaluate their performance on the same dataset using
consistent evaluation metrics and a common train/test split.

The project also explores hyperparameter tuning, training time,
model interpretability, and classification performance.

## 🎯 Objectives

- Train three classification algorithms on the same dataset.
- Use the same train/test split for a fair comparison.
- Tune at least one hyperparameter for each model.
- Evaluate accuracy, precision, recall, and F1-score.
- Generate confusion matrices for all three models.
- Compare training and tuning time.
- Recommend a suitable model based on experimental results.

## 📊 Dataset

**Dataset:** Breast Cancer Wisconsin Diagnostic Dataset

The dataset is available through Scikit-learn.

- Samples: 569
- Features: 30 numerical features
- Target classes: Malignant and Benign
- Problem type: Binary classification

## 🛠️ Technologies Used

- Python
- Pandas
- Matplotlib
- Scikit-learn
- Google Colab
- Jupyter Notebook

## 🤖 Algorithms Implemented

### 1. Decision Tree

A tree-based classification algorithm that makes predictions using
a sequence of feature-based decision rules.

Hyperparameter tuned: `max_depth`

### 2. Random Forest

An ensemble learning algorithm that combines multiple decision trees
to improve prediction robustness.

Hyperparameter tuned: `n_estimators`

### 3. Support Vector Machine (SVM)

A classification algorithm that identifies a decision boundary
between classes. An RBF kernel is used to model nonlinear boundaries.

Hyperparameter tuned: `C`

Feature standardization is performed within the SVM pipeline.

## 📈 Evaluation Metrics

All models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- Training and tuning time

Five-fold cross-validation is used for hyperparameter selection.

The dataset is split once into 80% training data and 20% testing data.
All three models use the same split.

## 🏆 Results and Model Comparison

The following results were observed in the experimental run.
Verify the values against the executed notebook before submission.

| Metric | SVM | Random Forest | Decision Tree |
|---|---:|---:|---:|
| Test Accuracy | 98.25% | 95.61% | 92.11% |
| Malignant Recall | 97.62% | 95.12% | 86.67% |
| Malignant F1-score | 97.62% | 93.98% | 88.16% |

SVM achieved the strongest reported performance in this experiment.
It also had the lowest observed training and tuning time.

These results apply to this experimental run and do not guarantee
the same ranking on other datasets or data splits.

## ⚙️ How to Run

1. Clone or download this repository.
2. Open the `.ipynb` notebook in Google Colab or Jupyter Notebook.
3. Install the required libraries if they are not already available:

   `pip install pandas matplotlib scikit-learn`

4. Run the notebook cells from top to bottom.
5. Review the model comparison table and confusion matrices.

The dataset is loaded directly from Scikit-learn, so no separate
dataset download is required.

## 💡 Key Learnings

- How to train and evaluate classification algorithms.
- Why using the same train/test split matters.
- How hyperparameter tuning affects model performance.
- How to interpret confusion matrices and evaluation metrics.
- Why accuracy alone is not sufficient for model selection.
- How to compare predictive performance with computational cost.

## ✅ Conclusion

The experiment compares Decision Tree, Random Forest, and SVM using
a consistent evaluation procedure.

SVM achieved the highest reported test accuracy and malignant-class
F1-score in this run. Therefore, it was the strongest candidate among
the three models for this particular experiment.

Further validation would be required before applying these findings
to real-world medical diagnosis.

## 👨‍💻 Project Information

**Project:** DS-6 Classification Algorithms Comparison

**Domain:** Machine Learning

**Language:** Python

**Framework:** Scikit-learn
