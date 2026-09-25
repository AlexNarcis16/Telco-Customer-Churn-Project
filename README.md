# Telco-Customer-Churn-Project
This is a Machine Learning project in Python whose objective is to predict if a customer will leave the telecommunications company based on contract details, including contract type, subscribed services, payment method, tenure and associated charges.

The database used for this project can be found on Kaggle (https://www.kaggle.com/datasets/blastchar/telco-customer-churn). It contains data of 7043 customers of a telecommunications company, such as demographic information (gender, seniority), customer account information (how long they have been customers of the company, contract, payment method) and services included in their contract (phone, internet, online security, tech support).

The project consists in two parts. The first part is EDA (Exploratory Data Analysis), where I checked the dataset for null values and outliers and created graphs that show the relationships between different variables. The second part is applying Machine Learning models such as Random Forest, XGBoost, CatBoost and Decision Trees to predict if a customer leaves or stays with the company. The most important libraries used: pandas, scikit-learn, matplotlib, xgboost, catboost.

The results from the below table show that the most efficient model overall applied on this dataset is CatBoost, although there are no major differences between models. F1-Scores around 0.53-0.58 show that nearly half of churn predictions are wrong, either missing customers who actually leave or flagging customers who stay. AUC-ROC values (0.68-0.71) confirm only moderate ability to distinguish between the two groups, suggesting these models would need further tuning before being reliable for real business decisions.

|     Model     | Accuracy | F1-Score | AUC-ROC |
|-------        |----------|----------|---------|
| Decision Tree |  0.7299  |  0.5297  |  0.6796 |
| Random Forest |  0.7804  |  0.5463  | 0.6909  |
|    XGBoost    |  0.7740  |  0.5679  | 0.7054  |
|    CatBoost   |  0.7868  |  0.5822  | 0.7141  |



