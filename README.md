# 📊 Student Performance Prediction

## 📌 Project Overview
This project is part of the **Elevvo Machine Learning Internship (Task 1)**. The objective is to analyze the factors influencing student academic performance and build a predictive model to estimate exam scores based on study hours, attendance, sleep habits, and parental involvement.

While the primary requirement was to implement **Linear Regression**, this repository goes further by benchmarking multiple algorithms and engineering a robust preprocessing pipeline to maximize accuracy.

## 📂 Dataset
* **Source:** Student Performance Factors (Kaggle).
* **Target Variable:** `Exam_Score`.
* **Key Features:** `Hours_Studied`, `Attendance`, `Sleep_Hours`, `Parental_Involvement`, `Access_to_Resources`.

## 🛠️ Tech Stack
* **Language:** Python 3.10+
* **Libraries:**
    * **Data Manipulation:** Pandas, NumPy
    * **Visualization:** Matplotlib, Seaborn
    * **Machine Learning:** Scikit-Learn
    * **Model Serialization:** Joblib

## ⚙️ Project Workflow
1.  **Data Cleaning:** Handled missing values (dropped nulls to ensure data integrity).
2.  **Exploratory Data Analysis (EDA):**
    * Analyzed correlations between study habits and grades.
    * Visualized the impact of socioeconomic factors (e.g., Family Income, Parental Education).
3.  **Preprocessing:**
    * **Scaling:** Applied `StandardScaler` to numerical features and `MinMaxScaler` to bounded variables.
    * **Encoding:** Used Label Encoding for categorical variables.
4.  **Modeling & Benchmarking:**
    * **Baseline:** Linear Regression.
    * **Complexity:** Polynomial Regression (Degree 2).
    * **Advanced Models:** Random Forest, Gradient Boosting, SVR, KNN.
5.  **Deployment:** Saved the best-performing model (`champion_model.pkl`) using Joblib for future inference.

## 📈 Key Findings
* **Study Hours vs. Scores:** Positive correlation confirmed, but diminishing returns observed after a certain threshold.
* **Attendance:** High attendance is a strong prerequisite for high scores (it sets the "floor" for performance).
* **Socioeconomic Impact:** Students with higher access to resources and parental involvement tend to have a higher median score, though individual motivation plays a significant role.

## 🚀 How to Run
1.  Clone the repository:
    ```bash
    git clone [https://github.com/YourUsername/student-performance-prediction.git](https://github.com/YourUsername/student-performance-prediction.git)
    ```
2.  Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3.  Run the Jupyter Notebook:
    ```bash
    jupyter notebook student-score-prediction.ipynb
    ```

## 🏆 Results
The models were evaluated using **R2 Score** and **RMSE**. The comparative analysis (found in the notebook) highlights which model offers the best balance between accuracy and generalizability.

---
*Elevvo Internship | Task 01 - Level 1*
