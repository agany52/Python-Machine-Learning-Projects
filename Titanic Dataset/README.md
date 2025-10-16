Project 2: Titanic Survival Prediction

🚢 Project Overview

This project tackles the classic Kaggle competition, "Titanic: Machine Learning from Disaster." The goal is to build a machine learning model that can predict whether a passenger on the Titanic survived or not, based on their personal data such as age, sex, class, etc.

This is a foundational project in supervised learning that demonstrates a complete, end-to-end data science workflow, from initial data cleaning and exploration to building and evaluating a predictive classification model. It serves as a practical application of the core concepts covered in the first course of Andrew Ng's Machine Learning Specialization.

workflow The Process

The project followed a structured data science methodology to ensure a robust and understandable outcome.

1. Data Loading & Initial Exploration:

The raw training and testing datasets were loaded into Pandas DataFrames.

An initial exploration was conducted using .info() and .describe() to understand the data types, identify missing values, and get a statistical summary of the numerical features.

2. Data Cleaning & Preprocessing:

Handling Missing Values: Null values in critical columns like Age and Embarked were addressed. The Age NaNs were filled with the median age of the dataset, and the single missing Embarked value was filled with the most common port of embarkation.

Dropping Unnecessary Columns: Features that were not useful for prediction, such as Ticket, Cabin, and Name, were dropped to simplify the model.

3. Feature Engineering:

Converting Categorical Features: Non-numerical columns like Sex and Embarked were converted into numerical representations using one-hot encoding so they could be used by the machine learning model.

4. Model Building & Training:

The preprocessed dataset was split into features (X) and the target variable (y, which is 'Survived').

The data was further split into a training set (80%) and a testing set (20%) using scikit-learn's train_test_split function.

A Logistic Regression model was chosen for this binary classification task. The model was trained on the training data.

5. Model Evaluation:

The trained model was used to make predictions on the unseen testing set.

The model's performance was evaluated by calculating the accuracy score, which measures the percentage of correct predictions.

💡 Key Skills Demonstrated

Supervised Learning: Building a model to predict a labeled outcome.

Classification: Specifically, a binary classification problem (Survived vs. Not Survived).

Data Cleaning: Handling missing data and irrelevant features.

Feature Engineering: Transforming raw data into a format suitable for modeling.

Model Evaluation: Assessing model performance with accuracy metrics.

Python Libraries: Proficient use of Pandas for data manipulation and Scikit-learn for building and evaluating the machine learning model.

📊 Results

The final Logistic Regression model achieved an accuracy of 80.45% on the test!
