# breast-cancer-prediction-ml_improved
 we will upgrade your project into a stronger ML project by adding: Cross-validation   XGBoost   Neural Network   Explainable AI



# Breast Cancer Prediction using Machine Learning

## Project Overview

This project builds and evaluates multiple machine learning models to predict whether a tumor is **benign or malignant** using the Breast Cancer dataset from Scikit-learn.

The goal is to compare different algorithms, analyze model performance, and explain predictions using **Explainable AI techniques (SHAP)**.

This project demonstrates a complete **end-to-end machine learning workflow**, including:

- Data preprocessing
- Model training
- Cross-validation
- Model comparison
- Explainable AI
- ROC curve analysis

---

# Dataset

Dataset used:

**Breast Cancer Wisconsin Dataset**

Source:
Scikit-learn built-in dataset

Features include:

- mean radius
- mean texture
- mean perimeter
- mean area
- concavity
- concave points
- symmetry
- fractal dimension

Target:
0 = benign
1 = malignant


Total samples:

569 tumors


---

# Machine Learning Models Used

The following models were trained and evaluated:

1. Logistic Regression
2. Random Forest
3. Support Vector Machine (SVM)
4. XGBoost
5. Neural Network (MLPClassifier)

---

# Model Evaluation Metrics

Models were evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC Curve
- AUC Score

These metrics are important in **medical classification problems**, where detecting malignant tumors is critical.

---

# Final Model Comparison

| Model | Accuracy | Precision | Recall | F1 Score |
|------|------|------|------|------|
| Logistic Regression | 0.965 | 0.959 | 0.986 | **0.973** |
| Random Forest | 0.956 | 0.959 | 0.972 | 0.966 |
| SVM | 0.930 | 0.921 | 0.972 | 0.946 |
| XGBoost | 0.947 | 0.946 | 0.972 | 0.959 |
| Neural Network | 0.965 | **0.986** | 0.958 | 0.972 |

Best model based on **F1 Score and AUC**:

Logistic Regression


---

# ROC Curve Comparison

The ROC curve evaluates how well each model distinguishes between benign and malignant tumors.

AUC scores:

| Model | AUC |
|------|------|
| Logistic Regression | **0.995** |
| Random Forest | 0.994 |
| Neural Network | 0.994 |
| XGBoost | 0.993 |
| SVM | 0.970 |

Higher AUC indicates better classification performance.

---

# Explainable AI (SHAP)

To understand **why models make predictions**, SHAP (SHapley Additive exPlanations) was used.

SHAP helps identify which features most influence the model’s decisions.

Top influential features:

- worst perimeter
- worst texture
- worst concave points
- worst area
- mean concave points

This improves **model interpretability**, which is important in healthcare applications.

---

# Project Workflow

Data Loading
↓
Data Preprocessing
↓
Train/Test Split
↓
Train Multiple ML Models
↓
Cross Validation
↓
Model Evaluation
↓
Explainable AI (SHAP)
↓
ROC Curve Analysis
↓
Final Model Comparison


---

# Technologies Used

Python

Libraries:

- scikit-learn
- pandas
- numpy
- matplotlib
- seaborn
- xgboost
- shap

---



---

# Future Improvements

Potential improvements include:

- Hyperparameter tuning
- Deep learning models
- Larger medical datasets
- Model deployment using Flask or FastAPI

---

# Author

**Gautami Patel**

Software Developer | Machine Learning Enthusiast

LinkedIn:
https://www.linkedin.com/in/gautami-p-3b5a88363/

GitHub:
https://github.com/gautamikpatel2612

---

# License

This project is open-source and available under the MIT License.
