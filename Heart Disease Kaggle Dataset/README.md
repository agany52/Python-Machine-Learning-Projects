Heart Disease Prediction & Analysis 🫀

📌 Project Overview

An exploratory data analysis and prediction model for heart disease presence. This project investigates the relationship between cardiovascular metrics (like chest pain type, cholesterol, and exercise-induced angina) and the presence of heart disease.

Key Objective: Can we accurately predict heart disease using a simple Logistic Regression model, and how do variables like Angina impact those predictions?

🛠️ Tech Stack

Language: Python

Libraries: Pandas, Scikit-Learn, Matplotlib, Seaborn

Tools: Jupyter Notebook

🔍 Key Insights & "The Angina Anomaly"

During the analysis, I discovered a counter-intuitive correlation in the dataset regarding Exercise Induced Angina (exang).

Typically, angina is a sign of heart disease.

In this dataset, patients with angina were statistically less likely to have the target heart disease label.

Hypothesis: This suggests a potential labeling issue in the dataset source or a specific subset of patients where angina acts as a differentiating factor against other conditions.

📊 Model Performance

I iterated on a Logistic Regression model:

Baseline: ~79% Accuracy

Feature Engineering (One-Hot Encoding): Improved to ~82% Accuracy

Threshold Tuning: Lowered decision threshold to 0.2 to maximize Recall, ensuring that we minimize False Negatives (missing a sick patient), even if it means slightly more false alarms.

📂 Project Structure

Heart_Disease_Analysis.ipynb: The main analysis and modeling code.
