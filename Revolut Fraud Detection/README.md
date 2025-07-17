Fraudulent Users Detection

File: Revolut_User_Fraud_Detection.ipynb

Overview: 

Detection of fraudulent users, where an account can be determined as fraudulent due to the primary reasons as account takeovers by hackers and payment fraud.

Key Features:

Data exploration and analysis of Revolut user and transaction data, including examining missingness, data types, and target variable distribution.
Exploratory Data Analysis (EDA) to identify patterns and trends in user and transaction attributes associated with fraudulent behavior. This involves analyzing categorical features (e.g., phone_country, kyc, currency, entry_method, state, merchant_category) and continuous features (e.g., birth_year, amount_usd) in relation to the is_fraud target.
Feature engineering, including:
Dummy Encoding of categorical variables.
Aggregation of transaction data at the user level within different time windows (7 and 30 days) for numerical, boolean, and ID features.
Decomposition of timestamps into various components (year, month, day, day of week, etc.).
Weight of Evidence (WoE) encoding for categorical variables.
Creating features like feat__transaction_number and feat__phone_country_count.
Data splitting into training, validation, and test sets based on a specific date to simulate a production environment.
Feature selection using a combination of feature importance (SelectKBest with f_classif) and feature clustering to identify relevant and non-collinear features.
Implementation and training of a machine learning model (XGBoost Classifier).
Model evaluation and comparison using the ROC-AUC metric on validation and test sets.
Hyperparameter tuning of the XGBoost model using RandomizedSearchCV, incorporating undersampling with RandomUnderSampler to address class imbalance.

Technologies:

Python,
Pandas,
Scikit-learn,
Scipy,
imb-learn,
XGBoost,

Expected Outcomes:

ML model capable of predicting the probability of a user being fraudulent. The goal is to identify users who are likely to engage in fraudulent activities based on their profile and transaction history.
Insights into the predictive power of various features related to user characteristics (e.g., country, KYC status, sign-in attempts), transaction details (e.g., currency, entry method, amount, state), and aggregated behavioural patterns (e.g., transaction counts, average transaction amounts over time).
Performance metrics of the XGBoost model, likely focusing on the ROC-AUC score, highlighting its effectiveness in distinguishing between fraudulent and non-fraudulent users. This will also involve evaluating the impact of hyperparameter tuning and undersampling on the model's performance.
Understanding of the challenges and limitations of fraud detection, particularly in an imbalanced dataset and in a dynamic environment where fraud patterns can evolve. This might include insights into the trade-offs between false positives and false negatives and the practical considerations of deploying such a model.
