Data Science Portfolio
===========================================================================

This repository contains two Jupyter notebooks for data science projects:

1. Amazon Stock Price Direction
2. Real Estate Engagement
3. TikTok Content Moderation
4. Employee Churn for HR Department

Project 1: Amazon Stock Price Direction
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

Project 2: Real Estate Engagement
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


Project 3: TikTok Content Moderation
---------------------------------------

File: classifying-claims-and-opinions-in-tiktok-content.ipynb

Overview:
This project focuses on developing a machine-learning model to classify TikTok video content into claims and opinions. The classification is crucial for content moderation and understanding user-generated content on the platform.

Key Features:
- Data preprocessing of TikTok video text data
- Exploratory data analysis of claims and opinions distribution
- Feature engineering for text data
- Implementation and training of machine learning models
- Model evaluation and performance assessment

Technologies:
- Python
- Pandas
- Scikit-learn
- Natural Language Processing (NLP) techniques

Expected Outcomes:
- A trained model for classifying TikTok content
- Insights into characteristics of claims vs. opinions in social media
- Performance metrics of the classification model

Project 4: Employee Churn Prediction
---------------------------------------------------

File: salifort-motors-predicting-employee-churn.ipynb

Overview:
This project aims to develop a predictive model for employee churn at Salifort Motors. The analysis will help in developing retention strategies and improving workforce planning.

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
