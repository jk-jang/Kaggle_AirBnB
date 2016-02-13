# AirBnB competition on Kaggle
Please download the data sets from the [Kaggle competition page](https://www.kaggle.com/c/airbnb-recruiting-new-user-bookings).

## Solution for Rank 23
1. Built a **Logistic Regression** model as the base classifier using the one-hot encoded features from sessions data to classify NDF vs non-NDF users (binary classifier). Code can be found in **_model_lr.R_**

2. Built an **XGBoost** model as the meta classifier using the raw features, the one-hot encoded features from sessions data and the logistic regression predictions along with some basic feature engineering to classify the users into the 12 countries (multiclass classifier). Code can be found in **_model_xgb.R_**

3. The model scored 0.88081 on the public LB ranked 89 and scored 0.88625 on the private LB ranked 23 using the NDCG metric.
