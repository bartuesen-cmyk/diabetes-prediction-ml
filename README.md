# Diabetes Prediction Using Machine Learning

IE413 Information Systems course assignment - Sabancı University

## 📋 Project Overview

This project implements a complete machine learning pipeline to predict diabetes using the Pima Indians Diabetes dataset. The analysis includes data preprocessing, feature scaling, model training, and comprehensive evaluation using multiple classification algorithms.

## 📊 Dataset

- **Source:** Pima Indians Diabetes Dataset
- **Samples:** 768 patients
- **Features:** 8 diagnostic measurements (Glucose, BMI, Age, Blood Pressure, etc.)
- **Target:** Binary classification (Diabetes: Yes/No)
- **Class Distribution:** 35% diabetic, 65% non-diabetic

## 🤖 Models Implemented

Three classification algorithms with parameter tuning:

- **Logistic Regression** (C=0.1, C=1.0)
- **K-Nearest Neighbors** (k=5, k=10)
- **Random Forest** (max_depth=5, max_depth=10)

## 📈 Results

| Model | Accuracy | Precision | Recall | F1-Score |
|-------|----------|-----------|--------|----------|
| Logistic Regression (C=0.1) | 0.688 | 0.565 | 0.481 | 0.520 |
| Logistic Regression (C=1.0) | 0.701 | 0.587 | 0.500 | 0.540 |
| KNN (k=5) | 0.753 | 0.660 | 0.611 | 0.635 |
| KNN (k=10) | 0.740 | 0.652 | 0.556 | 0.600 |
| Random Forest (depth=5) | 0.740 | 0.667 | 0.519 | 0.583 |
| **Random Forest (depth=10)** | **0.760** | **0.681** | **0.593** | **0.634** |

**Best Model:** Random Forest with max_depth=10 (76.0% accuracy)

## 🔍 Key Findings

- **Recall** is the most critical metric for diabetes prediction due to the severe consequences of false negatives (missing diabetic patients)
- Non-linear models (Random Forest, KNN) significantly outperformed Logistic Regression
- Parameter tuning showed measurable improvements across all model types
- Class imbalance (35% diabetic cases) affects model performance

## 🛠️ Technologies Used

- Python 3.9
- scikit-learn
- pandas
- NumPy
- matplotlib
- seaborn

## 📁 Files

- `esen_bartu_assg.ipynb` - Main Jupyter notebook with complete analysis
- `confusion_matrices.png` - Visualization of model performance

## 🚀 Future Improvements

1. Address class imbalance using SMOTE or class weight adjustment
2. Feature engineering: interaction terms and polynomial features
3. Hyperparameter optimization using GridSearchCV
4. Ensemble methods combining multiple models

## 👤 Author

Bartu Esen - Industrial Engineering, Sabancı University

---

*Assignment completed for IE413 - Information Systems (December 2025)*
