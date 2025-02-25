Loan Default Prediction Using Machine Learning
📌 Project Overview
This project focuses on predicting loan default risk using advanced machine learning models. The implementation follows a structured approach, from data preprocessing to model training and deployment via Flask API.

🚀 Key Features
Data Preprocessing: Handling missing values, encoding categorical variables, and feature scaling.
Exploratory Data Analysis (EDA): Data visualization and correlation analysis.
Feature Engineering: Creating meaningful features to improve accuracy.
Model Selection & Training: Using XGBoost, CatBoost, Random Forest, and Logistic Regression.
Model Evaluation: Comparing models using F2-score, recall, and confusion matrix.
Deployment: Implementing a Flask API and integrating it with ngrok for serving predictions.
Database Storage: Saving predictions in a SQLite database for historical analysis.
🔧 Setup & Installation
📌 Install Required Libraries
sh
Copy
Edit
pip install catboost shap category_encoders numerize torchsampler torchmetrics flask flask-ngrok
📌 Clone the Repository
sh
Copy
Edit
git clone https://github.com/your-username/Loan-Default-Prediction.git  
cd Loan-Default-Prediction  
📌 Run the Flask API
sh
Copy
Edit
python app.py  
📊 Data Preprocessing
✅ Handling Missing Values
Dropped or imputed missing values in critical columns.
✅ Encoding Categorical Variables
Used one-hot encoding and label encoding.
✅ Feature Scaling
Normalized numerical values for improved model performance.
✅ Handling Class Imbalance
Used scale_pos_weight in XGBoost and balanced class weights in other models.
🛠 Model Training & Evaluation
📌 Machine Learning Models Used
Random Forest
XGBoost
CatBoost
Logistic Regression
📌 Performance Metrics
Model	F2-Score (Train)	F2-Score (Test)	Recall (Train)	Recall (Test)
Random Forest	0.85	0.79	0.89	0.81
XGBoost	0.88	0.82	0.91	0.84
CatBoost	0.87	0.83	0.90	0.85
Logistic Regression	0.75	0.71	0.78	0.73
📌 Confusion Matrix & SHAP Analysis
Visualized confusion matrix to analyze false positives/negatives.
Used SHAP values for feature importance but faced runtime errors.
Solution: Researched multiple sources and adjusted model configurations.
🔥 Challenges Faced & Solutions
🛠 SHAP Runtime Error
Encountered issues due to high memory usage.
Solution: Optimized feature selection and adjusted SHAP calculations.
🛠 Torchsampler Issue in Jupyter Notebook
Installed torchsampler, but it failed to work in Google Colab.
Solution: Used WeightedRandomSampler as an alternative.
🛠 Flask API in Notebook
Issue: Running Flask inside Jupyter Notebook caused execution failures.
Solution: Used ngrok to create a tunnel for the Flask API.
🌍 Deployment
✅ Flask API
The model is deployed via Flask to handle user inputs and return predictions.
✅ Database Integration
SQLite Database stores past predictions.
✅ API Endpoints
/predict → Accepts input data and returns loan default probability.
/history → Retrieves stored predictions.
📌 Project Insights & Future Enhancements
✅ Insights from Data

Defaulting loans are correlated with credit score, income level, and past loan behavior.
XGBoost & CatBoost performed the best, but Random Forest also gave competitive results.
✅ Future Improvements

Optimize feature selection for better accuracy.
Deploy the model on cloud platforms (AWS, GCP).
Improve the Flask UI for a user-friendly experience.
👨‍💻 Author
Priyanka Joshi
📌 B.Tech CSE (AI & ML), Sir Padampat Singhania University
📌 Aspiring Data Scientist & AI Enthusiast

📜 License
This project is open-source under the MIT License.

🎯 Want to Contribute?
Pull requests and suggestions are welcome! 😊

# Important Libraries install
-!pip install catboost
-!pip install shap
-!pip install category_encoders
-!pip install numerize
-!pip install torchsampler
-!pip install torchmetrics
-!pip install flask flask-ngrok

#The implementation of the project follows these key steps:

Data Preprocessing: Handling missing values, encoding categorical variables, feature scaling.

Exploratory Data Analysis (EDA): Understanding data distribution and correlations.

Feature Engineering: Creating meaningful features to enhance prediction accuracy.

Model Selection & Training: Training models like XGBoost, CatBoost, Random Forest, and Logistic Regression.

Evaluation: Using metrics like F2-score, recall, and confusion matrix to compare models.

Deployment: Implementing a Flask API to serve predictions and storing results in a database.
