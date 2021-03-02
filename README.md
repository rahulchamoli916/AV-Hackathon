# AV-Hackathon

This contest proposed by the Analytics Vidya. Where the community of data science and machine learning practitioners and experienced peoples can participate. Now let's dive to the actual problem -

## Problem Statement

There is a company 'XYZ', which works as a financial company and providing various services like Finance, Insurance, Loans etc. The company have recently launched a new Insurance policy, and wants to know the tendency of existing customers and new customers to purchase that policy. If customer purchase, then it's a **lead** otherwise **no-lead**. So ultimately it's a binary classification case.

## The Task

The task at hand is, given a data-point (user's detail) model has to prdict the Response, whether it's a lead or not.

## Data

Data also provided by the Analytics Vidya, which is also present in the repository as -

**train.csv** - Containing the train data, including the class label as 'Response'.

**test.csv** - Actual test data, without any class label.

**sample_submission.csv** - Submission file format.

## Performance Metric

According to the organizers, Leaderboard can be decided by using 'roc-auc-score' as Performance Metric.

## EDA

The whole EDA regarding this project is available in the repository under **EDA.ipynb**.

## Feature Engineering

Since lots of feature in the dataset are 'Categorical features', so it's always good to try **One-hot encoding**, **Response coding**, **Label Encoding** and some other stuffs. I tried one-hot encong and label encoding. The performance is good for the label encoded features as compare to one-hot encoded features. And for the numerical features I kept them as it is. The entire EDA is also available in the repository under **LGBM model.ipynb**.

## Modeling

Since dataset is small so I tried all the major ML models like **Logistic Regression**, **Decision Tree**, **Random Forest**, **XGBoost**, **LightGBM**, and **CatBoost**. For my case LightGBM worked well, as compare to other models. LightGBM modeling is also present in the repository under the **LGBM model.ipynb**.

## Results

After submitting LightGBM model, I achieved 315th place out of 2363 entries on the Private Leaderboard. My scores are -

Private Leaderboard - 0.6700517236
Public Leaderboard - 0.6700070309
