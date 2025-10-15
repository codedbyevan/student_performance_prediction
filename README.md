# 🎓 Student Performance Prediction using Linear Regression

This project explores how various academic and lifestyle factors influence students' academic performance.  
Using a clean regression workflow, it predicts each student’s **Performance Index (10–100)** based on their study habits, past results, and daily routines.

---

## 📊 Dataset Overview

**Dataset:** [Student Performance Dataset](https://www.kaggle.com/datasets/nikhil7280/student-performance-multiple-linear-regression)  
**Records:** 10,000 students  
**Target Variable:** `Performance Index`

### Features
| Feature | Description |
|----------|-------------|
| **Hours Studied** | Total study hours per student |
| **Previous Scores** | Student’s previous test scores |
| **Extracurricular Activities** | Participation in extracurricular activities (`Yes`/`No`) |
| **Sleep Hours** | Average sleep hours per day |
| **Sample Question Papers Practiced** | Number of practice papers solved |

---

## 🧠 Objective

To build and evaluate a **regression model** that can accurately predict a student’s performance index using available academic and lifestyle features.

---

## ⚙️ Methodology

1. **Data Preprocessing**
   - Loaded dataset with Pandas.
   - Converted categorical features (e.g., *Extracurricular Activities*) into numeric values.
   - Checked for missing values and basic descriptive statistics.

2. **Exploratory Data Analysis (EDA)**
   - Correlation heatmap to identify relationships.

3. **Modeling**
   - Split dataset into **Train (80%)** and **Test (20%)** sets.
   - Trained a **Linear Regression** model using scikit-learn.
   - Evaluated with R², MAE, and RMSE metrics.

4. **Evaluation Metrics**
   | Metric | Result | Interpretation |
   |---------|---------|----------------|
   | **R² Score** | **0.989** | Explains 98.9% of variance — excellent fit |
   | **MAE** | **1.61** | Model is off by ~1.6 points on average |
   | **RMSE** | **2.02** | Typical prediction error ≈ 2 points |

5. **Visualizations**
   - Actual vs Predicted Performance (scatter)
   - Residual analysis
   - Feature–target fit plots
   - Coefficient importance visualization

---

## 🧩 Key Insights

- **Previous Scores** are the strongest predictor of future performance.
- **Hours Studied** also shows a strong positive correlation.
- **Sleep Hours** and **Practice Papers** have minor effects.
- Linear Regression performs exceptionally well on this dataset due to clear, linear relationships.

---

## 📈 Example Plots

| Visualization | Description |
|----------------|--------------|
| **Correlation Heatmap** | Reveals feature relationships |
| **Actual vs Predicted** | Model accuracy visualization |
| **Residual Plot** | Checks model error distribution |
| **Feature Fit Lines** | Shows model trends per feature |

---

## 🚀 Future Improvements

- Experiment with non-linear models (Random Forest, XGBoost)  
- Include more behavioral or demographic features  
- Apply cross-validation for more robust evaluation  
- Deploy the model as a simple web app using Streamlit  

---

## 🧰 Tech Stack

- **Python 3.10+**
- **Libraries:** pandas, numpy, matplotlib, seaborn, scikit-learn
- **Tools:** Jupyter Notebook / VS Code, GitHub
