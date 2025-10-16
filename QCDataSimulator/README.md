Lab Instrument QC Anomaly Detector

🎯 Project Overview

This project is an end-to-end demonstration of how unsupervised machine learning can be used to automatically detect anomalies in simulated Quality Control (QC) data from laboratory instruments. The goal is to identify subtle issues like spikes or data drift that could indicate an instrument is failing, allowing for predictive maintenance before it impacts real-world results.

This project is specifically designed to showcase a practical, industry-relevant application of data science skills for the biotechnology and healthcare sectors.

🛠️ Technical Stack

Language: Python

Libraries:

Pandas & NumPy for data manipulation and simulation.

Matplotlib for data visualization.

Scikit-learn for implementing the machine learning model.

🚀 Methodology

The project was executed in three main parts:

Part 1: Data Simulation

Since real QC data is proprietary, a realistic dataset was simulated from scratch. This involved:

Generating a baseline of "normal" QC data with random noise to mimic real-world variance.

Injecting two types of anomalies: a sudden point anomaly (spike) and a gradual contextual anomaly (drift).

Part 2: Anomaly Detection with Isolation Forest

An unsupervised machine learning approach was used to identify unusual data points without any prior labeling.

An Isolation Forest model was chosen for its effectiveness in identifying outliers.

The model was trained on the simulated data to learn the structure of "normal" behavior. It then assigned an anomaly score to each data point, flagging the most unusual ones.

Part 3: Hyperparameter Tuning for Optimal Performance

To find the best setting for the model, an automated tuning process was implemented.

A "ground truth" or "answer key" was created, as the anomalies were known from the simulation phase.

A loop was created to test a range of contamination values (the model's sensitivity).

The F1-Score was used to evaluate each model's performance, identifying the contamination value that provided the best balance of precision and recall.

📊 Results

The final, optimized model successfully identified both the sudden spike and the gradual drift in the data. The results are visualized below, with the detected anomalies highlighted in red. The tuning process demonstrated that a contamination value of [Enter the best value you found here] provided the most accurate results for this dataset.

(Pro-tip: Take a screenshot of your final plot, save it as final_plot.png, and upload it to your GitHub repository so it shows up here!)

🏃 How to Run

Clone this repository.

Ensure you have the required libraries installed (pandas, numpy, matplotlib, scikit-learn).

Run the qc_hyperparameter_tuner.ipynb notebook. The notebook contains all the code for simulation, tuning, and visualization.

<img width="1226" height="619" alt="image" src="https://github.com/user-attachments/assets/3a2442d5-3050-4120-b2c6-cda7994dcedd" />

