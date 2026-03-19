# California Housing Price Prediction - Machine Learning Project

This project builds a machine learning model to predict median house prices in California districts using demographic and housing data.

The project demonstrates a complete machine learning workflow including:

- Exploratory Data Analysis (EDA)
- Feature Engineering
- Preprocessing Pipelines
- Model Comparison
- Cross-Validation
- Hyperparameter Tuning
- Feature Importance Analysis
- Unsupervised Clustering (KMeans)

## Model Performance

| Model | MAE |
|------|------|
| Linear Regression | 49,645 |
| Decision Tree | 43,093 |
| Random Forest | 31,926 |
| Random Forest (Tuned) | **31,758** |

The final model is a tuned **Random Forest Regressor** with a Mean Absolute Error (MAE) of approximately **$31,758**.

## Dataset

California Housing dataset (housing.csv)

Each row represents a housing district and contains information about:

* location (longitude, latitude)
* housing characteristics
* population and households
* median income
* proximity to the ocean

Target variable:

median_house_value

## Project Structure

california_housing_project/
│
├── data/
│   └── housing.csv
│
├── notebooks/
│   └── ML_Housing_Notebook_Elza_Capar.ipynb
│
├── reports/
│   ├── ML_Housing_Report_Elza_Capar_en.pdf
│   └── ML_Housing_Report_Elza_Capar_se.pdf
│
├── requirements.txt
├── .gitignore
└── README.md

## Project Report

The written report is available in the **/reports** folder.

Two versions are included:

* **English version** – included for portfolio purposes so the project is accessible to an international audience
* **Swedish version** – the version submitted for the course assignment

All code, comments, and documentation in this repository are written in **English** to make the project easier to read and understand for a broader audience on GitHub.

## Machine Learning Workflow

The notebook follows a complete machine learning pipeline:

1. **Data Exploration (EDA)**  
   Understanding the dataset, distributions, correlations, and missing values.

2. **Feature Engineering**  
   Creating additional variables such as rooms_per_household and population_per_household.

3. **Data Splitting**  
   Dividing the dataset into training and testing sets.

4. **Preprocessing Pipeline**  
   Handling missing values, scaling numerical features, and encoding categorical variables using scikit-learn pipelines.

5. **Model Training and Comparison**  
   Training Linear Regression, Decision Tree, and Random Forest models.

6. **Cross-Validation**  
   Evaluating models using 5-fold cross-validation to obtain more reliable performance estimates.

7. **Hyperparameter Tuning**  
   Optimizing the Random Forest model using GridSearchCV.

8. **Model Evaluation**  
   Evaluating the final model using MAE and RMSE.

9. **Feature Importance Analysis**  
   Identifying which variables most influence housing price predictions.

10. **Unsupervised Learning**  
   Applying KMeans clustering to identify groups of housing areas.

## Python Version

Python 3.11.9

## Installation and Reproducibility

To reproduce the analysis in this project, follow the steps below.

1. Clone the Repository
- git clone https://github.com/elzacapar/california-housing-ml.git

3. Create a Virtual Environment
- On Windows:
python -m venv .venv
.venv\Scripts\activate

- On macOS or Linux:
python3 -m venv .venv
source .venv/bin/activate

3. Install Required Dependencies
- pip install -r requirements.txt

The notebook can be reproduced by running:

Restart & Run All
