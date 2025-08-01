# 🩺 SEPSIS Prediction and Data Analysis Using Machine Learning

This project aims to predict the onset of **Sepsis** using patient vitals and clinical data through various machine learning algorithms. The notebooks contain both **exploratory data analysis (EDA)** and **predictive modeling**, helping in early detection and prevention strategies.

---

## 📁 Project Structure

- **`SEPSIS.ipynb`** – Implements machine learning models for early prediction of sepsis.
- **`Analysis.ipynb`** – Performs data exploration and visualization to understand feature distributions and relationships.

---

## 📌 Problem Statement

Sepsis is a potentially life-threatening condition caused by the body's response to an infection. Timely detection is crucial for reducing mortality. In this project, we use patient data to:
- Analyze important indicators
- Build predictive models to identify sepsis-prone individuals

---

## 🧠 Techniques Used

### `Analysis.ipynb`:
- Data cleaning (NaN handling, null counts)
- Exploratory Data Analysis:
  - Distribution plots (Temperature, Heart Rate, Respiratory Rate, etc.)
  - Correlation matrix to detect multicollinearity
  - Sepsis case distribution
  - Feature trends over time

### `SEPSIS.ipynb`:
- Data preprocessing
- Model building using:
  - Logistic Regression
  - Decision Trees
  - Random Forest
  - Support Vector Machines
  - K-Nearest Neighbors
- Model evaluation:
  - Confusion Matrix
  - Accuracy, Precision, Recall, F1-score
  - ROC-AUC Curve

---

## 📊 Dataset Summary

- **Features:** Age, Gender, Heart Rate, Temperature, O2 Saturation, and other clinical metrics
- **Target:** SepsisLabel (0 - No Sepsis, 1 - Sepsis)
- **Preprocessing:** Handled missing values and normalized input features

---

## ✅ Results

| Model               | Accuracy | Precision | Recall | F1-Score |
|--------------------|----------|-----------|--------|----------|
| Logistic Regression|   ~0.89  |   High    |  High  |   High   |
| Decision Tree      |   ~0.86  |   High    |  Medium|   Medium |
| Random Forest      |   ~0.90  |   High    |  High  |   High   |
| SVM                |   ~0.87  |   High    |  Medium|   Medium |
| KNN                |   ~0.85  |   Medium  |  Medium|   Medium |

> Random Forest performed best in most metrics and showed robustness in both precision and recall.

---

## ⚙️ How to Run

1. Clone or download this repository
2. Open `SEPSIS.ipynb` and `Analysis.ipynb` in a Jupyter environment
3. Run all cells sequentially to replicate the results

---

## 🧾 Requirements

- Python 3.x
- Libraries:
  ```bash
  pandas
  numpy
  matplotlib
  seaborn
  scikit-learn
  ```

---

## 🔍 Insights

- Temperature, O2 saturation, and respiratory rate were strong indicators of sepsis.
- Early detection using machine learning can significantly help in triage systems in hospitals.


This project is for academic and educational purposes only and should not be used for real-time clinical decisions.
