Medical Insurance Cost Prediction

📌 Project Overview
This project aims to predict medical insurance charges based on patient features (age, BMI, smoking status, etc.). I conducted a full machine learning pipeline, moving from a baseline linear model to advanced ensemble techniques, ultimately achieving a high-performing and robust predictive model.
📊 Dataset Features

- Age: Age of primary beneficiary.
- Sex: Insurance contractor gender (female, male).
- BMI: Body mass index, providing an understanding of body weight relative to height.
- Children: Number of children covered by health insurance / Number of dependents.
- Smoker: Smoking status (yes, no).
- Region: The beneficiary's residential area in the US.
- Charges: Individual medical costs billed by health insurance (Target Variable).

⚙️ Workflow & Methodology

1. Exploratory Data Analysis (EDA)

- Identified significant "clusters" in the data related to smoking status and BMI.
- Detected heteroscedasticity in the baseline model, where prediction error increased for higher charges.

2. Model Evolution
   I tested three different algorithms to find the most accurate and stable model:

- Linear Regression: Used as a baseline; struggled with non-linear relationships.
- XGBoost Regressor: High performance (R^2: 0.8554), but required careful tuning.
- Random Forest Regressor (Champion): Achieved the best balance of accuracy and stability.

3. Optimization & Validation

- Cross-Validation: Implemented 5-fold CV to prove the model's reliability across different data slices.
- Hyperparameter Tuning: Used GridSearchCV to optimize parameters like max_depth and min_samples_split.

💡 Key Insights (Feature Importance)
The final Random Forest model identified the top drivers of medical costs:

1. Smoker Status: By far the most influential factor.
2. BMI: Critical predictor, especially for individuals in the obese range.
3. Age: Predictable linear increase in costs over time.

Tech Stack

- Language: Python
- Libraries: Pandas, Scikit-Learn , Matplotlib, Seaborn , ML Models
- Tools: VS Code
