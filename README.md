# Waze-User-Behavior-Regression-Modeling-Project
***Please note**: If the files do not load promptly, kindly give it a moment or try refreshing the page. GitHub occasionally takes a few seconds to render files, especially if they are content-rich. Your patience is appreciated!*


## Introduction
Join me as I explore and analyze of user behavior on Waze, a navigation app that helps millions navigate their journeys. While Waze is an essential tool for many, the challenge lies in keeping users engaged and preventing churn. Churn is defined as users uninstalling or ceasing to use the app. This project aims to build a binomial logistic regression model to uncover key drivers of churn and provide actionable insights to enhance user retention.
## Business Problem/Context
Waze’s free navigation app empowers drivers around the world to reach their destinations efficiently and safely, supported by a vibrant community of users, map editors, and partners. To ensure continued growth, Waze is tackling the challenge of monthly user churn, defined as users uninstalling the app or ceasing to use it.

This project is a critical component of Waze’s broader strategy to increase retention and engagement. By developing a **prediction model**, Waze aims to identify at-risk users, understand why and when users churn, and uncover key factors driving churn.

The ultimate goal is to enable Waze to proactively engage users at risk of churning with targeted interventions, thereby improving user retention, optimizing the user experience, and supporting the company’s growth objectives. 
## Methodology
The analysis began with exploratory data analysis (EDA) to understand key features, assess class balance, and identify patterns in user behavior. Missing data and outliers were addressed, and features were prepared for modeling. To ensure the robustness of the logistic regression model, key assumptions such as the linear relationship between features and log-odds were checked, and multicollinearity among predictors was assessed.

A binomial logistic regression model was then developed to predict user churn and identify key drivers. Stratified splits were used to maintain the representativeness of the dataset, and class imbalance was considered during model building. Finally, the model was evaluated using performance metrics such as accuracy, precision, recall, and F1-score, with confusion matrices visualized to better understand the strengths and weaknesses of predictions.
## Challenges and Resolutions
One of the primary challenges in this analysis was addressing outliers in the data, which had the potential to distort the model's predictions. To resolve this, outliers were identified and capped at the 95th percentile to minimize their impact while preserving the integrity of the dataset. Additionally, explaining the model results to non-technical stakeholders was challenging, but was overcome by breaking them down into simple, business-relevant terms.
## Results
The logistic regression model achieved an accuracy of 83%, but the recall for identifying churners was only 6%, indicating the model struggles to correctly classify at-risk users. The confusion matrix highlighted a significant number of false negatives, meaning many churners were incorrectly predicted as retained.

Activity days emerged as the most important predictor, showing a very strong negative correlation with churn. Features like km_per_driving_day had minimal impact on the model’s predictions, suggesting that such features were less relevant for understanding churn behavior.

These results underscore the need for improving the model’s ability to identify churners through techniques like addressing class imbalance, adding more features, and exploring alternative models.
## Next Steps
- Add engagement metrics to improve churn prediction.
- Try alternative models like Random Forest or Gradient Boosting.
- Test strategies like daily streaks or notifications to boost retention.
-  Fix class imbalance with oversampling, undersampling, or class weights.
## Tools and Packages Used
- Python, Git, Google Sheets
- Git 2.47.1
- Python version 3.11.0
- Pandas version 1.4.2
- Matplotlib version 3.5.1
- Seaborn version 0.11.2
## Sharing and Collaboration
The shared Jupyter Notebook and Executive Summary are not only a demonstration of my Data Analytics capabilities but also an invitation to inspire and guide others in their Data Analysis endeavors. Your engagement and feedback enrich the collective learning experience, contributing to a dynamic Data Analytics community.
**PS*. The dataset used in this study does not accurately reflect the user behavior within the Waze navigation app.*
