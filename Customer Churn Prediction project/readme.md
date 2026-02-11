📉 Customer Churn Prediction: Strategic Retention Model
A Machine Learning approach to identifying high-risk customers and maximizing Customer Lifetime Value (CLV).

🎯 Project Objective
It costs 5x more to acquire a new customer than to retain an existing one. This project provides a predictive pipeline that flags "At-Risk" customers with 86% accuracy, allowing the marketing team to intervene with targeted discounts before the customer leaves.

🛠 Feature Engineering & Preprocessing
To improve model performance, the raw data was transformed via:

One-Hot Encoding: Converted categorical variables (Smoker, Region, Sex) into binary vectors.

Standard Scaling: Scaled numerical features (Age, BMI) to a mean of 0 and variance of 1 to ensure the model isn't biased by large units.

Target Analysis: Checked for class imbalance (important for Churn) to ensure the model doesn't just "guess" the majority class.

🏆 Model (Classification)
I compared multiple algorithms to find the best balance between speed and sensitivity:

Logistic Regression: The interpretable baseline.

Random Forest: To capture complex non-linear interactions.

XGBoost: The champion for high-precision ranking.

Evaluation Metrics (Beyond Accuracy)
In churn, Accuracy is a trap. If 90% of people stay, a model that says "everyone stays" is 90% accurate but 0% useful. Instead, I focused on:

Recall: "How many of the actual churners did we find?" (Crucial for not missing at-risk people).

Precision: "When we flag a customer, how often are we right?" (Ensures we don't give discounts to happy customers).

ROC-AUC: A measure of how well the model separates "Stayer" from "Leaver."
