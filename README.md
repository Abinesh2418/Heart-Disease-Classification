# ❤️ Heart Disease Classification

This project uses machine learning to predict the presence of heart disease in patients based on clinical parameters. It leverages Python-based libraries to build, evaluate, and improve classification models. The goal is to support early diagnosis and medical decision-making.
---
## 🧠 About the Project
This notebook looks into using various Python-based machine learning and data science libraries to build a classification model capable of predicting whether or not someone has heart disease based on their medical attributes.

1. **Problem Definition**
   
   Given clinical parameters about a patient, can we predict whether or not they have heart disease?
3. **Data**
   
   The dataset used in this project is a structured heart disease dataset containing patient medical records with 14 attributes. It is based on the Cleveland Heart Disease dataset and is commonly used for binary classification tasks in healthcare machine learning.
   The dataset includes features such as age, sex, chest pain type, resting blood pressure, cholesterol levels, fasting blood sugar, electrocardiographic results, maximum heart rate, and others. The target variable indicates the presence (`1`) or absence (`0`) of heart disease.
5. **Evaluation**
     
   If we can reach **85% accuracy** at predicting heart disease during the proof of concept, we'll consider it a success.
7. **Features & Data Dictionary**
     

| Feature     | Description |
|-------------|-------------|
| age         | Age in years |
| sex         | Sex (1 = male; 0 = female) |
| cp          | Chest pain type (0–3) |
| trestbps    | Resting blood pressure (mm Hg) |
| chol        | Serum cholesterol (mg/dl) |
| fbs         | Fasting blood sugar > 120 mg/dl (1 = true; 0 = false) |
| restecg     | Resting electrocardiographic results (0–2) |
| thalach     | Maximum heart rate achieved |
| exang       | Exercise induced angina (1 = yes; 0 = no) |
| oldpeak     | ST depression induced by exercise |
| slope       | Slope of the peak exercise ST segment (0–2) |
| ca          | Number of major vessels (0–3) colored by flourosopy |
| thal        | Thalium stress result (1,3 = normal; 6 = fixed defect; 7 = reversible defect) |
| target      | Presence of heart disease (1 = yes; 0 = no) |

---

## 📁 Project Structure

Heart-Disease-Classification/
├── Dataset/
│ └── heart.csv
├── heart_disease_analysis.ipynb
├── requirements.txt
└── README.md

## 🧠 Project Workflow Summary

This project involves building a machine learning model to predict the presence of heart disease using various patient attributes. The following steps were carried out:

### 📌 1. Data Preprocessing
- Loaded the heart disease dataset from a CSV file.
- Handled missing values (if any) and verified data integrity.
- Converted categorical features to numerical (if required).
- Split the dataset into training and testing sets using `train_test_split`.
- Scaled the feature values for better model performance.

### 🤖 2. Model Building
- Implemented and compared multiple classification models:
  - `RandomForestClassifier`
  - `KNeighborsClassifier`
  - `LogisticRegression`
- Created a utility function `fit_and_score()` to train each model and evaluate their accuracy on the test set.

### 🔍 3. Hyperparameter Tuning
- Performed **RandomizedSearchCV** and **GridSearchCV** to find the best hyperparameters for `LogisticRegression` and `RandomForestClassifier`.
- Explored a wide range of parameters such as `C`, `solver`, `n_estimators`, `max_depth`, and `min_samples_leaf` for improved accuracy.

### 📊 4. Model Evaluation
- Evaluated model performance using key metrics:
  - Accuracy
  - Precision
  - Recall
  - F1-Score
- Used `cross_val_score` to validate the consistency of the model using k-fold cross-validation (k=5).

### ✅ 5. Final Model Selection
- Chose the best-performing model based on a balance of evaluation metrics.
- Achieved high accuracy and reliable performance in predicting heart disease from clinical data.

---

