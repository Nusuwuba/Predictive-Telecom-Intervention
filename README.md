Predictive Telecom Intervention

## Overview
This repository contains a machine learning pipeline and business strategy designed to transform a standard telecom churn prediction model into a proactive intervention engine. It addresses a 49.5% baseline churn rate heavily driven by hardware fatigue. 

By identifying customers approaching an 11-month device age cliff, this targeting engine allows telecom providers to proactively offer subsidized handset upgrades conditional upon a 12-month contract renewal.

*Note: This project was originally developed as a final submission for the GCI World 2026 competition. It builds upon a foundational data science tutorial by expanding the exploratory data analysis (EDA), engineering new features, and optimizing advanced ensemble methods against the tutorial's baseline.*

## Business Impact
* **Predictive Accuracy:** The final XGBoost model achieved 64.2% accuracy on highly noisy human behavioral data, representing a 14.8% absolute improvement over random baseline guessing.
* **Return on Investment (ROI):** At a $150 hardware subsidy per retained user, the intervention pays for itself in 3 months.
* **Projected Revenue:** The deployment of this targeting engine is estimated to save $1.2M annually per 10,000 users.

## Repository Contents
* `churn_prediction_engine.ipynb`: The main Jupyter Notebook containing data preprocessing, exploratory data analysis, feature engineering, and model evaluation (Logistic Regression, Random Forest, XGBoost).
* `report.pdf`: The executive slide deck detailing the strategic hypothesis, ML methodology, and financial quotation.
* `requirements.txt`: The software dependencies required to reproduce the environment.

## Reproducing the Project
To respect data privacy, the raw `100k_customer_records.csv` dataset is not hosted in this repository. 

1. Clone this repository: `git clone <your-repo-url>`
2. Install the required dependencies: `pip install -r requirements.txt`
3. Place the dataset in the root directory.
4. Run the Jupyter Notebook to train the models and generate the evaluation metrics.

## Technical Stack
* **Data Processing & EDA:** Python, Pandas, NumPy
* **Machine Learning:** Scikit-learn, XGBoost
* **Visualization:** Matplotlib, Seaborn