Fraudulent Users Detection

File: DoorDash_Fraudulent_User_Detection.ipynb

Overview:

Detection of fraudulent users on the DoorDash platform, focusing primarily on account takeovers and payment fraud. The project aims to build a machine learning model that can effectively identify fraudulent consumer accounts requiring deactivation, thereby reducing financial losses and improving platform security.

Key Features:

Data Exploration and Analysis
Performed detailed Exploratory Data Analysis (EDA) to understand user and transaction data characteristics, evaluate missingness, feature distributions, and the relationship of variables to the target label (is_fraudulent). Key observations included dataset imbalance and strong signals from variables such as email_address_age_days and per_day_transactions.

Feature Engineering

Applied Weight of Evidence (WoE) encoding to handle categorical variables effectively, particularly those with high cardinality or sparsity. Transformed and cleaned data by imputing missing values (-999 for numerical, 'MISSING' for categorical). Created new features or enhanced existing ones to improve signal strength in classification.

Data Preparation

Split dataset into training, validation, and test sets to emulate a production-like modeling pipeline and prevent data leakage. Ensured appropriate data types for modeling and handled imbalance through undersampling techniques.

Feature Selection

Employed SelectKBest with f_classif to rank feature importance based on their statistical relevance to the fraud label. Compared multiple feature set sizes (top 10, 20, and all features); all features were retained due to cumulative predictive value.

Modeling

Used XGBoost Classifier as the primary model due to its robustness and ability to handle imbalanced datasets. Built a baseline model, followed by hyperparameter tuning using RandomizedSearchCV in conjunction with RandomUnderSampler to optimize performance.

Evaluation

Assessed model using ROC-AUC on train, validation, and test splits. Analyzed Precision-Recall trade-offs across thresholds on the validation set. Estimated financial benefit (Net Value) of deploying the model by comparing it against a no-detection baseline scenario.

Technologies:

Python,
Pandas,
Scikit-learn,
Scipy,
Imbalanced-learn (imblearn),
XGBoost,
Matplotlib / Seaborn,

Expected Outcomes:

A production-ready ML model capable of accurately predicting the probability of a user being fraudulent, enabling proactive deactivation of high-risk accounts. Identification of key behavioral and account-related indicators for fraud, such as email age and transaction volume. Performance benchmarking focused on ROC-AUC, with insights into the impact of hyperparameter tuning and class imbalance correction. Real-world implications and strategic insights for fraud detection in imbalanced and evolving environments, including cost-benefit analysis and deployment considerations.
