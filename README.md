🎓 Student Performance Prediction
📌 Overview
This project predicts whether a student will pass or fail based on various academic and behavioral features using a Random Forest Classifier. The aim is to identify students at risk and enable timely academic interventions.

We use a dataset that includes features such as absences, weekly study time, tutoring support, and parental involvement. The model is trained and evaluated using scikit-learn tools, with key metrics like accuracy, precision, recall, and a confusion matrix heatmap.

📂 Dataset
File: 8. Student Performance Prediction.csv

Source: Uploaded directly in Google Colab

Target Variable: Pass (1 = Pass, 0 = Fail)

Label Creation: A new Pass column is derived from GPA values:

GPA >= 2.0 → Pass (1)

GPA < 2.0 → Fail (0)

📊 Selected Features
The following features were used for training the model:

Absences: Number of days the student was absent

StudyTimeWeekly: Hours spent studying per week

Tutoring: Whether the student receives tutoring (1 = Yes, 0 = No)

ParentalSupport: Whether the student receives parental support (1 = Yes, 0 = No)

🧠 Model Methodology
🛠️ 1. Data Preparation
Dataset loaded and preprocessed in Google Colab.

Binary classification target (Pass) generated from GPA.

🔍 2. Feature Selection
Focused on meaningful academic and support-related features.

No unnecessary or high-dimensional features included for simplicity.

🤖 3. Model Building
Model: RandomForestClassifier (scikit-learn)

Reason: Handles mixed data types well and provides high accuracy with minimal tuning.

Split: 70% training / 30% testing using train_test_split.

📈 4. Evaluation
Confusion Matrix visualized using a heatmap (Seaborn).

Metrics used:

Accuracy

Precision

Recall

📌 Sample Output
makefile
Copy
Edit
Accuracy: 0.85
Precision: 0.84
Recall: 0.86
📊 Confusion Matrix is plotted to visually interpret classification performance.

📦 Requirements
Install the required libraries using:

bash
Copy
Edit
pip install pandas seaborn matplotlib scikit-learn
🧪 How to Run
Upload the CSV file to Colab using:

python
Copy
Edit
from google.colab import files
uploaded = files.upload()
Follow the steps to train and evaluate the model (as provided in the Python script).

View the printed metrics and the plotted confusion matrix heatmap.

📜 License
This project is open-source and free to use for academic and non-commercial purposes.
