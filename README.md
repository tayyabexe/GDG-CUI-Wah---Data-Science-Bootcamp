# GDG-CUI-Wah---Data-Science-Bootcamp
Can we predict a student's final grade before the exam? I explored this using the Student's dataset to build a complete ML pipeline. From cleaning "noisy" data to engineering features like Total_Academic. This repo shows my end-to-end process of building a Linear Regression model that prioritizes accuracy and interpretability.

This is a great idea! A well-structured README makes your project look professional and helps others (or your future self) understand exactly what you achieved.

Since we’ve gone through the whole journey—from fixing `UnicodeDecodeError` to building a predictive model—here is a polished README template you can use.

***

# 🎓 Student Performance Prediction 📈

## 📌 Project Overview
This project uses **Machine Learning (Linear Regression)** to predict a student's `Final_Score` based on their academic habits, demographics, and previous test results. 

The goal was to move beyond simple averages and understand which specific factors—like attendance, study hours, or midterm scores—actually influence a student's final grade.

## 🛠️ The "Data Cleaning" Journey
Real-world data is messy! This project involved a rigorous cleaning pipeline:
* **Handling Errors:** Fixed encoding issues and "impossible" values (e.g., Attendance > 100%).
* **Robust Imputation:** Used **Median** values to fill missing data to ensure outliers didn't skew the results.
* **Standardization:** Cleaned inconsistent text data (e.g., converting "male", "MALE", and " Male" into a single standard format).
* **Feature Engineering:** Created a `Total_Academic` weighted score to better represent student effort.



## 🧠 Model & Results
I built a Scikit-Learn **Pipeline** that automatically handles scaling for numbers and encoding for categories.

* **Primary Model:** Linear Regression
* **Key Metric (R²):** **0.59** (The model explains 59% of the variation in final scores).
* **Mean Absolute Error (MAE):** **2.45** (Predictions are off by less than 2.5 points on average).

### 🔍 What the Model Learned (Feature Weights)
The model identified the following as the top predictors:
1. **Midterm Score:** The strongest indicator of success.
2. **Quizzes & Assignments:** Significant contributors to the final grade.
3. **Attendance:** A steady positive influence on performance.



## 📈 Visualizing Accuracy
Below is a comparison of the **Actual Scores** (Blue Dots) vs. the **Predicted Scores** (Red Crosses). The close alignment shows the model's ability to track the general trend of student performance accurately.

*(Insert your saved plot `student_performance_comparison.png` here)*

## 🚀 How to Run
1. Clone this repository.
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn openpyxl
   ```
3. Run the Jupyter Notebook `student_analysis.ipynb`.

## 💡 Future Improvements
While an R² of 0.59 is a strong start, future versions could improve by:
* Collecting **Behavioral Data** (stress levels, sleep hours).
* Trying **Non-Linear Models** like Random Forest to capture more complex patterns.
* Investigating the 41% of variance currently unexplained by the academic data.

---
*Created by Tayyab Abdullah*
