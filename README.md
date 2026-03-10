{\rtf1\ansi\ansicpg1252\cocoartf2706
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Helvetica;\f1\froman\fcharset0 Times-Roman;}
{\colortbl;\red255\green255\blue255;\red0\green0\blue0;}
{\*\expandedcolortbl;;\cssrgb\c0\c0\c0;}
\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0

\f0\fs24 \cf0 # Breast Cancer Prediction using Machine Learning\
\
## Project Overview\
\
This project builds and evaluates multiple machine learning models to predict whether a tumor is **benign or malignant** using the Breast Cancer dataset from Scikit-learn.\
\
The goal is to compare different algorithms, analyze model performance, and explain predictions using **Explainable AI techniques (SHAP)**.\
\
This project demonstrates a complete **end-to-end machine learning workflow**, including:\
\
- Data preprocessing\
- Model training\
- Cross-validation\
- Model comparison\
- Explainable AI\
- ROC curve analysis\
\
---\
\
# Dataset\
\
Dataset used:\
\
**Breast Cancer Wisconsin Dataset**\
\
Source:\
Scikit-learn built-in dataset\
\
Features include:\
\
- mean radius\
- mean texture\
- mean perimeter\
- mean area\
- concavity\
- concave points\
- symmetry\
- fractal dimension\
\
Target:\
\pard\pardeftab720\partightenfactor0

\f1 \cf0 \expnd0\expndtw0\kerning0
\outl0\strokewidth0 \strokec2 0 = benign\
1 = malignant\
\
\
Total samples:\
\
569 tumors\
\
\
---\
\
# Machine Learning Models Used\
\
The following models were trained and evaluated:\
\
1. Logistic Regression\
2. Random Forest\
3. Support Vector Machine (SVM)\
4. XGBoost\
5. Neural Network (MLPClassifier)\
\
---\
\
# Model Evaluation Metrics\
\
Models were evaluated using:\
\
- Accuracy\
- Precision\
- Recall\
- F1 Score\
- ROC Curve\
- AUC Score\
\
These metrics are important in **medical classification problems**, where detecting malignant tumors is critical.\
\
---\
\
# Final Model Comparison\
\
| Model | Accuracy | Precision | Recall | F1 Score |\
|------|------|------|------|------|\
| Logistic Regression | 0.965 | 0.959 | 0.986 | **0.973** |\
| Random Forest | 0.956 | 0.959 | 0.972 | 0.966 |\
| SVM | 0.930 | 0.921 | 0.972 | 0.946 |\
| XGBoost | 0.947 | 0.946 | 0.972 | 0.959 |\
| Neural Network | 0.965 | **0.986** | 0.958 | 0.972 |\
\
Best model based on **F1 Score and AUC**:\
\
Logistic Regression\
\
\
---\
\
# ROC Curve Comparison\
\
The ROC curve evaluates how well each model distinguishes between benign and malignant tumors.\
\
AUC scores:\
\
| Model | AUC |\
|------|------|\
| Logistic Regression | **0.995** |\
| Random Forest | 0.994 |\
| Neural Network | 0.994 |\
| XGBoost | 0.993 |\
| SVM | 0.970 |\
\
Higher AUC indicates better classification performance.\
\
---\
\
# Explainable AI (SHAP)\
\
To understand **why models make predictions**, SHAP (SHapley Additive exPlanations) was used.\
\
SHAP helps identify which features most influence the model\'92s decisions.\
\
Top influential features:\
\
- worst perimeter\
- worst texture\
- worst concave points\
- worst area\
- mean concave points\
\
This improves **model interpretability**, which is important in healthcare applications.\
\
---\
\
# Project Workflow\
\
Data Loading\
\uc0\u8595 \
Data Preprocessing\
\uc0\u8595 \
Train/Test Split\
\uc0\u8595 \
Train Multiple ML Models\
\uc0\u8595 \
Cross Validation\
\uc0\u8595 \
Model Evaluation\
\uc0\u8595 \
Explainable AI (SHAP)\
\uc0\u8595 \
ROC Curve Analysis\
\uc0\u8595 \
Final Model Comparison\
\
\
---\
\
# Technologies Used\
\
Python\
\
Libraries:\
\
- scikit-learn\
- pandas\
- numpy\
- matplotlib\
- seaborn\
- xgboost\
- shap\
\
---\
\
\
\
---\
\
# Future Improvements\
\
Potential improvements include:\
\
- Hyperparameter tuning\
- Deep learning models\
- Larger medical datasets\
- Model deployment using Flask or FastAPI\
\
---\
\
# Author\
\
**Gautami Patel**\
\
Software Developer | Machine Learning Enthusiast\
\
LinkedIn:\
https://www.linkedin.com/in/gautami-p-3b5a88363/\
\
GitHub:\
https://github.com/gautamikpatel2612\
\
---\
\
# License\
\
This project is open-source and available under the MIT License.}