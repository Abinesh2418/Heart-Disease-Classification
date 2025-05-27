# ❤️ Heart Disease Classification

This project uses machine learning to predict the presence of heart disease in patients based on clinical parameters. It leverages Python-based libraries to build, evaluate, and improve classification models. The goal is to support early diagnosis and medical decision-making.
---
## 🧠 About the Project
This notebook looks into using various Python-based machine learning and data science libraries to build a classification model capable of predicting whether or not someone has heart disease based on their medical attributes.

1. **Problem Definition**
   Given clinical parameters about a patient, can we predict whether or not they have heart disease?
2. **Data**
   The dataset used in this project is a structured heart disease dataset containing patient medical records with 14 attributes. It is based on the Cleveland Heart Disease dataset and is commonly used for binary classification tasks in healthcare machine learning.
   The dataset includes features such as age, sex, chest pain type, resting blood pressure, cholesterol levels, fasting blood sugar, electrocardiographic results, maximum heart rate, and others. The target variable indicates the presence (`1`) or absence (`0`) of heart disease.
3. **Evaluation**  
   If we can reach **85% accuracy** at predicting heart disease during the proof of concept, we'll consider it a success.
4. **Features & Data Dictionary**  

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


