# Loan Default Prediction Using Machine Learning  

## 📌 Project Overview  
This project focuses on **predicting loan default risk** using advanced machine learning models. The implementation follows a structured approach, from **data preprocessing** to **model training** and **deployment via Flask API**.  

## 🚀 Key Features  
- **Data Preprocessing**: Handling missing values, encoding categorical variables, and feature scaling.  
- **Exploratory Data Analysis (EDA)**: Data visualization and correlation analysis.  
- **Feature Engineering**: Creating meaningful features to improve accuracy.  
- **Model Selection & Training**: Using **XGBoost, CatBoost, Random Forest, and Logistic Regression**.  
- **Model Evaluation**: Comparing models using **F2-score, recall, and confusion matrix**.  
- **Deployment**: Implementing a **Flask API** and integrating it with **ngrok** for serving predictions.  
- **Database Storage**: Saving predictions in a **SQLite database** for historical analysis.  

---

## 🔧 Setup & Installation  

### 📌 Install Required Libraries  
```sh
pip install catboost shap category_encoders numerize torchsampler torchmetrics flask flask-ngrok

git clone https://github.com/Priyanka12joshi/Default-Loan-Prediction-Using-ML.git  
cd Loan-Default-Prediction  
