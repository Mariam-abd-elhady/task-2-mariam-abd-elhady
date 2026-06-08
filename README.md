# 🧠 Stroke Prediction Analysis

## Project Overview
This project focuses on analyzing health data and predicting whether a patient will have a stroke using machine learning techniques. The dataset contains various medical features such as age, hypertension, heart disease, glucose levels, BMI, and other factors that influence stroke risk.

## Dataset
The `healthcare-dataset-stroke-data.csv` dataset was used, which contains patient health records from various sources. The data includes:
- Demographic information (gender, age, residence type)
- Medical history (hypertension, heart disease)
- Lifestyle factors (work type, smoking status, marital status)
- Health metrics (average glucose level, BMI)
- Target variable (stroke occurrence)

## Data Processing Steps
1. Handling missing values (BMI column)
2. Encoding categorical variables (gender, work_type, ever_married, residence_type, smoking_status)
3. Feature scaling (BMI standardization)
4. Outlier detection and removal using IQR
5. Splitting data into training and testing sets

## Machine Learning Models Used
The following classification models were implemented and evaluated:
- Logistic Regression
- Gaussian Naive Bayes
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest
- Extra Trees
- AdaBoost
- Gradient Boosting
- Hist Gradient Boosting
- XGBoost
- CatBoost
- LightGBM

## Evaluation Metrics
The models were evaluated using:
- Accuracy
- Precision
- Recall
- F1-Score
- Balanced Accuracy
- ROC-AUC
- Confusion Matrix
- Precision-Recall Curve

## Results

| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|-------|----------|-----------|--------|-----------|---------|
| SVM | ~96% | 0.71 | 0.11 | 0.19 | 0.843 |
| XGBoost | ~96% | 0.71 | 0.11 | 0.19 | 0.843 |
| Logistic Regression | ~95% | 0.00 | 0.00 | 0.00 | 0.834 |
| KNN | ~95% | 0.00 | 0.00 | 0.00 | 0.711 |
| Random Forest | ~95% | 0.00 | 0.00 | 0.00 | 0.833 |
| Decision Tree | ~95% | 0.00 | 0.00 | 0.00 | 0.833 |
| Naive Bayes | ~37% | 0.07 | 0.98 | 0.12 | 0.843 |

## Key Insights
The high-performing models (SVM and XGBoost) showed good predictive capability for stroke prediction, with strong ROC-AUC scores (0.84). However, due to severe class imbalance (95% no stroke, 5% stroke), most models struggled with recall for the minority class. Naive Bayes achieved the highest recall (98%) but with very low precision. SVM and XGBoost provided the best balance between precision and recall.

## Requirements
- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- tqdm
- xgboost
- lightgbm
- catboost

## Author
Mariam Abd Elhady

