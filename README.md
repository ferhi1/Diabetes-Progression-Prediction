# Diabetes Progression Prediction

## Project Overview
This project predicts diabetes progression in patients based on clinical features using machine learning models. The goal is to provide insights into disease progression and compare the performance of different regression models.

## Dataset
The dataset is from **scikit-learn** (`load_diabetes`) and contains clinical data collected from 442 patients.

- **Features:**
  - age: age of the patient
  - sex: gender of the patient
  - bmi: body mass index
  - bp: average blood pressure
  - s1 – s6: blood serum measurements
- **Target:** Disease progression metric one year after baseline measurement
- **Samples:** 442

## Machine Learning Models Used
1. **Linear Regression** – basic regression model to predict target values.
2. **Ridge Regression** – regularized linear regression to reduce overfitting.
   - Hyperparameter: `alpha = 0.001`
3. **Random Forest Regressor** – ensemble method to improve prediction accuracy.
   - Hyperparameters: `max_depth=10`, `n_estimators=500`

## Results
| Model                  | R² Score |
|------------------------|----------|
| Linear Regression      | 0.516    |
| Ridge Regression       | 0.517    |
| Random Forest Regressor| 0.534    |

**Observation:** Random Forest performs the best with the highest R² score, indicating better prediction of diabetes progression.

## Installation
1. Make sure **Python 3.x** is installed.
2. Install required libraries:
```bash
pip install pandas scikit-learn
