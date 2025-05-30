Portfolio
===========================================================================

This repository contains notebooks for data science projects:

1. Fraudulent Users Detection
2. A/B Testing with Python
3. Amazon Stock Price Direction
4. Real Estate Engagement
5. Customer Churn Prediction

Project 1: Fraudulent Users Detection
---------------------------------------

File: Revolut_User_Fraud_Detection.ipynb

Overview:
Detection of fraudulent user, where an account can be determined as fraudulent due to the primary reasons as account takeovers by hackers and payment fraud.

Key Features:
- Data exploration and analysis of Revolut user and transaction data, including examining missingness, data types, and target variable distribution.
- Exploratory Data Analysis (EDA) to identify patterns and trends in user and transaction attributes associated with fraudulent behavior. This involves analyzing categorical features (e.g., phone_country, kyc, currency, entry_method, state, merchant_category) and continuous features (e.g., birth_year, amount_usd) in relation to the is_fraud target.
- Feature engineering, including:
    * Dummy Encoding of categorical variables.
    * Aggregation of transaction data at the user level within different time windows (7 and 30 days) for numerical, boolean, and ID features.
    * Decomposition of timestamps into various components (year, month, day, day of week, etc.).
    * Weight of Evidence (WoE) encoding for categorical variables.
    * Creating features like feat__transaction_number and feat__phone_country_count.
- Data splitting into training, validation, and test sets based on a specific date to simulate a production environment.
- Feature selection using a combination of feature importance (SelectKBest with f_classif) and feature clustering to identify relevant and non-collinear features.
- Implementation and training of a machine learning model (XGBoost Classifier).
- Model evaluation and comparison using the ROC-AUC metric on validation and test sets.
- Hyperparameter tuning of the XGBoost model using RandomizedSearchCV, incorporating undersampling with RandomUnderSampler to address class imbalance.

Technologies:
- Python
- Pandas
- Scikit-learn
- Scipy
- imb-learn
- XGBoost

Expected Outcomes:
- ML model capable of predicting the probability of a user being fraudulent. The goal is to identify users who are likely to engage in fraudulent activities based on their profile and transaction history.
- Insights into the predictive power of various features related to user characteristics (e.g., country, KYC status, sign-in attempts), transaction details (e.g., currency, entry method, amount, state), and aggregated behavioral patterns (e.g., transaction counts, average transaction amounts over time).
- Performance metrics of the XGBoost model, likely focusing on the ROC-AUC score, highlighting its effectiveness in distinguishing between fraudulent and non-fraudulent users. This will also involve evaluating the impact of hyperparameter tuning and undersampling on the model's performance.
- Understanding of the challenges and limitations of fraud detection, particularly in an imbalanced dataset and in a dynamic environment where fraud patterns can evolve. This might include insights into the trade-offs between false positives and false negatives and the practical considerations of deploying such a model.

Project 2: A/B Testing with Python
---------------------------------------

File: AB Testing Email Sign-Up.ipynb

Overview:
Evaluated the impact of changing the colour of the sign-up button. Compared the sign-up rates for the original & new button & determining if this seemingly minor design change could lead to a significant improvement in user conversions.

Key Features:
- Data Exploration and Analysis: Analyzing pre-test and test data, including daily visitor counts and sign-up rates.
- Hypothesis Formulation: Defining the null and alternative hypotheses for the A/B test.
- Experiment Design: Determining key parameters such as significance level (alpha), statistical power, minimum detectable effect (MDE), and calculating the required sample size and experiment duration.
- Validity Threat Assessment: Performing an AA test to ensure group comparability and a Sample Ratio Mismatch (SRM) check using the Chi-Square test to validate the randomization algorithm.
- Statistical Inference: Applying Chi-Squared and T-Tests for proportions to compare the sign-up rates of the control and treatment groups.
- Confidence Interval Analysis: Calculating and interpreting confidence intervals for the difference in sign-up rates to understand the range of potential improvement.
- Launch Decision: Making a data-driven recommendation based on the statistical significance and practical impact of the experiment results.

Technologies:
- Python
- Pandas
- SciPy
- statsmodels
- seaborn

Expected Outcomes:
- Determination of the impact of button color on sign-up rates: A clear conclusion on whether changing the sign-up button color from blue to green has a statistically significant impact on the sign-up rate.
- Quantification of the lift (if any) in sign-up rate: A measurement of the percentage increase or decrease in sign-up rate observed in the treatment group compared to the control group.
- Assessment of the experiment's validity: Confirmation that the experiment design and execution were sound, based on the AA test and SRM check results.
- Recommendation for future action: A data-backed decision on whether to implement the green button or maintain the original blue button.
- Insights into user behavior: Potential insights into how a seemingly small design change can influence user conversion.

Project 3: Amazon Stock Price Direction
---------------------------------------

File: Stock_Price_Direction.ipynb

Overview:
The project focuses on creating a machine learning algorithm designed to forecast the directional movement of Amazon's stock price. The model aims to predict whether the price will rise or fall by analysing historical stock data. This predictive capability could prove invaluable for traders seeking to make well-informed investment decisions.

Key Features:
- Data exploration and analysis of historical Amazon stock prices.
- Feature engineering, including calculating moving averages and price ranges.
- Implementation and training of classical machine learning models (Logistic Regression, Decision Tree, Random Forest, Gradient Boosting) and a deep learning model (Feedforward Neural Network).
- Model evaluation and comparison using the AUC metric on validation and test sets.
- Feature importance analysis to identify key drivers of stock price direction.

Technologies:
- Python
- Pandas
- Scikit-learn
- Keras
- Tensorflow

Expected Outcomes:
- ML capable of predicting the direction of Amazon stock price movement.
- Insights into the predictive power of various features (e.g., trading volume, moving averages).
- Performance metrics of the different models, highlighting the best-performing approach for this task.
- Understanding of the challenges and limitations of predicting stock price movements.

Project 4: Real Estate Engagement
---------------------------------------

File: Property_Click_Prediction.ipynb

The project aims to develop a machine learning model that predicts the number of interactions (clicks or views) a property will receive within a specific timeframe of its activation on a real estate platform. By analyzing historical property data and interaction patterns, the model strives to forecast property engagement, which can be valuable for real estate businesses aiming to optimize property listings and marketing strategies.

Key Features:
- Data exploration and preprocessing of property features (e.g., size, location, amenities) and interaction timestamps.
- Feature engineering, including calculating time-based features and handling categorical variables.
- Implementation and training of classical machine learning models (Linear Regression, Decision Tree, Random Forest, XGBoost) and potentially a deep learning model.
- Model evaluation and comparison using metrics such as Root Mean Squared Error (RMSE) and R-squared.
- Feature importance analysis to understand the key factors influencing property interactions.
- Handling imbalanced datasets for classification tasks (predicting interaction categories).

Technologies:
- Python
- Pandas
- Scikit-learn
- XGBoost
- Keras
  
Expected Outcomes:
- A machine learning model capable of predicting the number of interactions a property will receive.
- Insights into the predictive power of various property features and their impact on user engagement.
- Performance metrics of different models, highlighting the most accurate approach for this task.
- Understanding of the challenges and limitations of predicting property interactions in the real estate market.

Project 5: Employee Churn Prediction
---------------------------------------------------

File: https://github.com/mbajdman/Data-Science-Portfolio/blob/main/Customer%20Churn/Customer_Churn_Prediction.ipynb

Overview:
This project aims to develop a predictive model for customer churn. The analysis will help in developing retention strategies and improving workforce planning.

Key Features:
- Exploration of employee data to identify churn factors
- Data preprocessing and cleaning
- Feature engineering from employee data
- Implementation and training of machine learning models for churn prediction
- Model evaluation and performance assessment

Technologies:
- Python
- Pandas
- Scikit-learn
- Data visualization libraries (e.g., Matplotlib, Seaborn)

Expected Outcomes:
- A trained model for predicting employee churn
- Insights into factors contributing to employee turnover
- Recommendations for improving employee retention

Usage Instructions:
-------------------

For both notebooks:
1. Ensure all required libraries are installed
2. Load the respective datasets
3. Run the notebook cells sequentially
4. Interpret results and model outputs

Note: These notebooks require a Jupyter environment (e.g., Jupyter Lab, Google Colab) and appropriate datasets to run successfully.

For any questions or issues, please contact the repository maintainer.
