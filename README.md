# Machine_Learning_To_Predict_Customer_Personality
This is mini project from Rakamin Academy. The goal of this project is predict customer personality to boost marketing campaign by using machine learning. It helps company to analyze and understand their customer personality or behavior. So they can retargetting their business based on customer segmentation.

## Overview
 - Dataset is obtained from [Kaggle](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis) 
 - This data contain data from customer like income, marital status, year birth, total kids, goods that customer buy, and etc
 
## Data Processing
 - I using feature engineering to mmake column conversion rate from `total transaction` divided by `number of web visit per month`. After that I create the segmentation    of customer's age.
 - Then I did standardization (standard scaler) to the feature because we are going to use machine learning for classification the customer
 
 ## Data Modelling
 - By analyze Elbow Method and Silhouette Score we can get the optimal N-Cluster from K-Means Clustering algorithm
 - The optimal N-Cluster from this modelling is 4
 
 ## Interpretation
 - From the result of clustering we can get 4 segmentation of customer.
 - First segmentation is `risk of churn`. This customer have the lowest income and total transaction but have high number web visit
 - Second segmentation is `low spender`. This customer have low income and total transaction. They have low number web visit too
 - Third segmentation is `medium spender`. This customer have higher income and total transaction than low spender. But quite high response to marketing campaign
 - Forth segmentation is `high spender`. This customer have the highest income and total transaction. But have low number web visit. They have the highest conversion        rate too 
