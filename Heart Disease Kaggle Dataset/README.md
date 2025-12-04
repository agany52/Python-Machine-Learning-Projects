🫀 Heart Disease Risk Predictor

A machine learning application that predicts the likelihood of heart disease in patients based on 13 clinical features. Built with Python, Scikit-Learn, and Streamlit.

🎯 Project Goal

To build a diagnostic tool that prioritizes clinical safety (high Recall) over raw accuracy. As a phlebotomist transitioning into data science, I recognized that in a medical screening context, a False Negative (missing a sick patient) is far worse than a False Positive.

🛠️ Tech Stack

Model: Random Forest Classifier (Optimized for Recall)

App: Streamlit (Web Interface)

Data Processing: Pandas & NumPy

Validation: 5-Fold Cross-Validation

🧠 Key Features

Recall Optimization: The model's decision threshold was tuned from 0.5 to 0.3. This improved the detection of sick patients (Recall) from 75% to 90%.

Data Leakage Fix: Identified and removed ~700 duplicate rows from the original UCI dataset that were artificially inflating accuracy scores to 99%.

Interactive UI: Allows clinicians to input vitals (BP, Cholesterol, EKG) and receive real-time risk assessments.

🚀 How to Run Locally

Clone the repository.

Install dependencies:

pip install pandas scikit-learn streamlit joblib


Run the app:

streamlit run streamlit_app.py

🌐 Deployment (Streamlit Cloud)

This app is set up for easy deployment on Streamlit Community Cloud:

Prepare Requirements: Ensure a requirements.txt file exists in the repository with the necessary libraries (streamlit, pandas, scikit-learn, joblib, numpy).

Push to GitHub: Upload the code (streamlit_app.py, heart_disease_rf_model.pkl, requirements.txt) to a GitHub repository.

Deploy:

Go to Streamlit Community Cloud and log in.

Connect your GitHub account.

Select your repository and the main file (streamlit_app.py).

Click Deploy!

📊 Model Performance (Test Set)

Accuracy: ~82%

Recall (Sensitivity): ~90% (at 0.3 threshold)

Precision: ~78%
📂 Project Structure

Heart_Disease_Analysis.ipynb: The main analysis and modeling code.
