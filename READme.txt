Predicting Heart Attack Risk Using Machine Learning

Author: Divya Reddy Konda
Date: 04/18/2025
Programming Language: Python 3.12.7

Dependencies:
numpy
pandas
matplotlib
seaborn
scikit-learn
shap
xgboost              
jupyterlab           
ipykernel

Project Overview:
This project focuses on predicting heart attack risk using machine learning techniques based on clinical, demographic, and lifestyle-related data. The study involves building and evaluating multiple classification models, interpreting results with SHAP (SHapley Additive Explanations), and identifying key risk factors to support preventive cardiology.

Objective:
To develop a predictive model that can identify individuals at risk of heart attack using supervised machine learning methods, and to explain the model’s decisions through interpretable AI techniques.

Dataset:
- Source: Kaggle
- Link: https://www.kaggle.com/datasets/iamsouravbanerjee/heart-attack-prediction-dataset
- Records: 8,763 patients
- Features: 26 (demographics, lifestyle, clinical history)
- Target: Heart attack risk (0 = no risk, 1 = at risk)

Models Used:
- Logistic Regression
- Naive Bayes
- Decision Tree
- AdaBoost
- Random Forest
- Bagging Classifier

Each model was evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- AUC (ROC)

Model Interpretation:
SHAP (SHapley Additive Explanations) was used to interpret feature importance and visualize how individual variables impacted risk predictions.

Note:
The results shown in the initial presentation were based on temporary, preliminary runs. After reprocessing the dataset and tuning the models, the final evaluation metrics were updated. The results presented in the final report reflect the most accurate and up-to-date outcomes.

Key Findings:
- Top risk factors: Triglycerides, exercise hours, age, sedentary time, cholesterol, BMI, heart rate
- Best-performing model: Random Forest (based on precision and AUC)
- Class imbalance affected recall across most models, suggesting a need for resampling or cost-sensitive learning in future work.