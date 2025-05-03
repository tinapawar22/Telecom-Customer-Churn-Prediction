# Telecom-Customer-Churn-Prediction


Problem Statement
In the highly competitive telecom industry, retaining existing customers is significantly more cost-effective than acquiring new ones. This project focuses on identifying high-value prepaid customers at risk of churn in the Indian and Southeast Asian markets, where prepaid usage dominates. The goal is to build predictive models that can help telecom operators proactively retain such customers and reduce revenue leakage.

Business Objective
Predict churn of high-value customers using past behavior data.
Enable telecom firms to take corrective retention actions.
Identify key drivers of churn to inform strategic decisions.

 
 Project Approach
1. Data Understanding
Dataset contains customer-level usage and recharge data over 4 months.
Months are encoded as 6 (June) to 9 (September).


2. Data Preparation
Feature Engineering: Created derived features (e.g., recharge ratio, average usage).
High-Value Customer Filtering: Top 30% customers by average recharge in months 6 & 7.
Churn Tagging: Customers with zero usage (calls & data) in month 9 were tagged as churners.
Dimensionality Reduction: Used PCA to handle high-dimensional feature space.



3. Handling Class Imbalance
Applied SMOTE (Synthetic Minority Oversampling Technique) to balance the classes as churners were underrepresented.



4. Model Building
Built and evaluated multiple classification models:
Logistic Regression
Random Forest

Evaluated using metrics like Recall, Precision, F1-Score, and ROC-AUC to prioritize catching churners.



5. Interpretability
Trained a separate Logistic Regression model without PCA to identify key features influencing churn.




--Key Outcomes
Achieved significant improvement in identifying churners using recall-focused metrics.

Identified top predictors such as drop in recharge amount, data usage, and outgoing call minutes.

Enabled actionable insights for customer retention strategies.


 
--Tools & Technologies:
Python, Pandas, NumPy, Matplotlib, Seaborn

Scikit-learn for modeling, PCA, SMOTE, and evaluation
