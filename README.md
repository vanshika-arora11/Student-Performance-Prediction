# 🎓 Student Performance Prediction

## 📖 Project Description

This project aims to predict whether a student will **pass** or **fail** based on academic behavior and support factors. The model leverages a supervised learning approach using a **Random Forest Classifier**, offering interpretable and accurate predictions. The goal is to assist educators and institutions in identifying at-risk students early and enabling data-driven interventions.

---

## 📁 Dataset Information

- **File Name:** `8. Student Performance Prediction.csv`
- **Target Variable:** `Pass`
- **Label Definition:**
  - GPA ≥ 2.0 → **Pass** (1)
  - GPA < 2.0 → **Fail** (0)

---

## 🔍 Features Used

| Feature             | Description                                      |
|---------------------|--------------------------------------------------|
| `Absences`          | Number of school days missed                    |
| `StudyTimeWeekly`   | Hours spent studying per week                   |
| `Tutoring`          | Access to tutoring services (0 = No, 1 = Yes)   |
| `ParentalSupport`   | Parental academic support (0 = No, 1 = Yes)     |

---

## 🧠 Methodology

### 1. Data Preparation
- Dataset uploaded via `google.colab.files`.
- Created a binary `Pass` column derived from the GPA score.

### 2. Feature Selection
- Selected key features contributing to academic success.
- Focused on simplicity and interpretability.

### 3. Model Building
- **Algorithm:** `RandomForestClassifier`
- **Reason for Choice:** High accuracy, robustness, and ability to handle both categorical and numerical data.
- **Data Split:** 70% for training, 30% for testing (`train_test_split`).

### 4. Evaluation
- **Confusion Matrix:** Visualized using a heatmap (Seaborn).
- **Metrics Used:**
  - **Accuracy:** Overall correctness of the model
  - **Precision:** Proportion of predicted passes that were correct
  - **Recall:** Proportion of actual passes identified correctly

---

## 📈 Results (Example Output)

```plaintext
Accuracy: 0.85
Precision: 0.84
Recall: 0.86

