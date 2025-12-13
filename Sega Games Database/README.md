🎮 Strategic Portfolio Analysis (Sega Games Database)

This repository contains the Python (Jupyter Notebook) code for a project that analyzes the strategic direction of Sega's game portfolio, focusing on platform saturation and quality control.

The goal was to provide data-backed insights on where to focus development resources (PC vs. Mobile) by analyzing over 1,400 historical game releases.

💡 Key Strategic Insights

Insight

Finding

Business Recommendation

The Strategic Pivot

The highest volume of recent game releases is on PC (391) and iOS (119), not legacy consoles.

Confirm investment focus has successfully transitioned from hardware to high-volume software platforms.

PC Quality Volatility

PC titles exhibit the highest volatility in User Scores, fluctuating wildly between hits and flops.

Implement intensive pre-release QA and project selection rigor for the high-risk/high-reward PC portfolio.

Project Goal

To use a hybrid data pipeline (Python + Power BI) to move beyond "gut feeling" and generate clear, strategic recommendations for optimizing the game development portfolio.

🛠️ Technical Solution Summary

Data Cleaning: Used Python (Pandas) to programmatically clean the raw dataset, which involved complex tasks like grouping "long-tail" platforms and stripping special characters from developer and genre fields.

Data Modeling: The cleaned data was structured for analysis and imported into Power BI.

Executive Storytelling: A dashboard was built in Power BI to visualize platform saturation (Pie Chart) and track quality trends over time (Line Chart). Custom DAX measures were implemented to track metrics like Average User Score by platform.

⚙️ How to Run the Notebook

The notebook (Sega_Games_Database.ipynb) handles the data cleaning portion.

Download the Notebook: Download the Jupyter Notebook file directly from this repository.

Install Dependencies:

pip install pandas kagglehub


Data Access: The notebook uses the kagglehub library to automatically download the necessary dataset (joebeachcapital/sega-games).

Run the Notebook: Open the notebook in Jupyter or Google Colab and execute the cells sequentially. This will produce a clean CSV file (SegaGames_CLEAN.csv) ready for import into Power BI.

About the Author

Alec Gany is a Mathematics B.S. graduate focusing on Data Analytics. This project demonstrates strong skills in hybrid data engineering (Python for cleaning, Power BI for visualization) to solve real-world strategic business problems.
