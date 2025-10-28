## ElectrolAIte
ElectrolAIte is a machine learning framework for predicting activity coefficients and osmotic coefficients in aqueous electrolyte solutions.
Using advanced regression algorithms such as XGBoost, LightGBM, and ExtraTrees, ElectrolAIte demonstrates how artificial intelligence can reproduce complex thermodynamic behaviors typically modeled through virial expansions or empirical correlations.

#Project Overview

This project automates:

Loading and cleaning experimental electrolyte data,

Identifying unique electrolytes through their virial coefficients,

Training and comparing different machine learning regressors,

Visualizing predicted vs. experimental thermodynamic properties.

During comparative testing, XGBoost (XGBRegressor) emerged as the most performant algorithm, providing the most accurate and stable predictions.
This implementation showcases what an optimized, hyperparameter-tuned XGBoost model can achieve for chloride electrolyte systems.

#Key Features

Automated data preprocessing (format normalization, missing value handling)

Unique electrolyte identification using virial coefficients (Beta(0), Beta(1), C(phi), Beta(2))

High-performance regression modeling for:

Activity coefficient (γ)

Osmotic coefficient

Comprehensive visualizations of predicted vs. actual data


#Machine Learning Backbone

The algorithm used is XGBoost, the most accurate performer



#Workflow

Data Import – Load electrolyte property data from Excel database 

Cleaning & Preprocessing – Fill missing names, unify numeric formats

Electrolyte Identification – Generate a unique electrolyte key from virial parameters

Model Training – Predict γ and osmotic coefficients vs. molality

Visualization – Plot predicted and experimental data for each electrolyte


🧩 Example Output

Each plot shows:

Predicted vs. actual activity coefficients (γ)

Predicted vs. actual osmotic coefficients
as functions of molality (mol/kg) for each electrolyte.



🧪 Dependencies
pandas
numpy
matplotlib
seaborn
scikit-learn
xgboost
lightgbm
