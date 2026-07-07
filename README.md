CodeAlpha_DiseasePrediction

Predicts whether a breast tumor is Malignant or Benign using Logistic Regression, Random Forest, and SVM, based on diagnostic measurements from patient tissue samples.

Problem Statement

Given a set of numeric features computed from digitized images of breast tissue (cell radius, texture, smoothness, concavity, symmetry, etc.), classify whether the tumor is malignant or benign. Early, accurate diagnosis support like this is a common real-world application of classification models in healthcare.

Dataset

Wisconsin Breast Cancer Diagnostic Dataset — loaded directly from sklearn.datasets.load_breast_cancer().


569 patient records
30 numeric features per record (mean, standard error, and "worst" values for 10 cell nucleus measurements)
Binary target: 0 = Malignant, 1 = Benign


Approach


Loaded and inspected the dataset, checked class balance
Explored correlations between key features and diagnosis
Split data into train/test sets (80/20, stratified)
Scaled features using StandardScaler (for Logistic Regression and SVM)
Trained and compared three models:

Logistic Regression
Random Forest (200 trees, max depth 8)
SVM (RBF kernel)



Evaluated each model using Accuracy, Precision, Recall, F1-Score, and ROC-AUC
Visualized results with confusion matrices, ROC curves, and feature importance
Saved the best-performing model as a .pkl file


Results

ModelAccuracyPrecisionRecallF1-ScoreROC-AUCfill in from your results_df outputfill infill in

Best model: fill in — e.g. "Random Forest, ROC-AUC 0.99"

Tools & Libraries

Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, Joblib

How to Run


Open disease_prediction_colab.ipynb in Google Colab
Runtime → Run all
Charts and metrics display inline below each cell
Run the last cell to download generated files (dataset CSV, results, charts, saved model)


Files in this Repo


disease_prediction_colab.ipynb — full notebook with code and outputs
README.md — this file


Internship Context

This project was completed as part of the CodeAlpha Machine Learning Internship (Task 4: Disease Prediction from Medical Data).
