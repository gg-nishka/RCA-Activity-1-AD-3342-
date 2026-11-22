# Student Marks Prediction using Multiple Linear Regression

## Activity 1 – Regression and Classification Algorithms (CIE 2)
Submission GitHub ID: https://github.com/complexiota.
## 1. Project Overview
This project uses **Multiple Linear Regression** to predict a student's marks based on study hours and attendance. The goal is to understand how more than one numerical feature can influence a continuous output (marks).

## 2. Problem Statement
Predict a student's marks using:
- **Study Hours** – number of hours spent studying
- **Attendance** – attendance percentage

**Target:** Marks (predicted score out of 100)

## 3. Dataset
A small synthetic dataset was created for this activity with 50 student records.

| Column | Description | Type |
|---|---|---|
| `Study_Hours` | Daily study hours | Numerical input feature |
| `Attendance` | Attendance percentage | Numerical input feature |
| `Marks` | Student marks | Continuous target |

The dataset is provided in `student_marks_prediction_dataset.csv` in this repository. Since it is synthetic, it is intended for learning and demonstration only—not for real student evaluation.


## 4. Tools and Libraries
- Python
- Google Colab / Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Statsmodels (for VIF)

## 5. Activity Steps
1. Load the dataset and inspect sample rows and summary statistics.
2. Check for missing values and explore the data.
3. Plot feature relationships and a correlation heatmap.
4. Calculate the multiple linear regression coefficients manually for a small sample using the normal equation.
5. Train and compare a single-feature regression model (Study Hours) with a multiple-feature model (Study Hours and Attendance).
6. Evaluate the multiple-feature model using MAE, MSE, RMSE, R², and Adjusted R².
7. Plot predicted vs actual marks and examine residuals.
8. Check multicollinearity using VIF.
9. Predict marks for a new student example.

## 6. Multiple Linear Regression Equation
The general equation is:

`Marks = b0 + b1(Study_Hours) + b2(Attendance)`

Where:
- `b0` = intercept
- `b1` = coefficient of Study Hours
- `b2` = coefficient of Attendance

The fitted values of the intercept and coefficients are obtained from the model in the notebook.


## 7. Evaluation Metrics
- **MAE:** Average absolute difference between actual and predicted marks.
- **MSE:** Average of squared prediction errors.
- **RMSE:** Square root of MSE, expressed in marks.
- **R²:** Indicates how well the model explains variation in marks compared with a mean-based prediction.
- **Adjusted R²:** R² adjusted for the number of features used.


## 8. Conclusion
This activity demonstrates how Multiple Linear Regression can use study hours and attendance together to estimate student marks. The results are based on a synthetic dataset and a simple linear model, so the predictions are estimates and should not be used to make real academic decisions.


## 9. Repository Files
- `student_marks_prediction_dataset.csv` – dataset used for the activity
- `README.md` – project description and activity summary
- Notebook – code, calculations, visualisations, model evaluation, and prediction (upload the notebook to this repository)


## How to Run
1. Open the notebook in Google Colab.
2. Upload `student_marks_prediction_dataset.csv` when prompted or place it in the Colab working directory.
3. Run the notebook cells from top to bottom.

