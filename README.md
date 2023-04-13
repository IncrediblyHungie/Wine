Wine Quality Prediction


Business Problem and Stakeholders

The business problem we aim to solve is predicting a wine's potential rating to produce higher quality wines, leading to a more desirable product and increased sales. The stakeholders include vineyard owners, winemakers, wine distributors, and retailers who want to understand the factors contributing to wine quality and make informed decisions to improve their products.

Data Source

The dataset is sourced from Kaggle and is related to red variants of Spanish wines. The dataset describes several popularity and description metrics, exploring their effect on wine quality. The dataset can be used for classification or regression tasks. The classes are ordered and not balanced (i.e., the quality ranges from 5 to 4 points). The task is to predict either the quality of wine or the prices using the given data.

Data Description

The dataset contains information about the wine's winery, wine name, year, rating, number of reviews, country, region, price, type, body, and acidity. The dataset has a total of 11 features, including both categorical and numerical variables.

Analytical Insights

Price vs. Rating Correlation: The price and rating have a correlation of 0.51, indicating a moderate positive relationship. This means that as the price of the wine increases, its rating tends to increase as well. The heatmap and the plot support this finding.

![download](https://user-images.githubusercontent.com/123442350/231897309-dff91d8a-2a74-4f23-9c44-609ec2144b5f.png)

Rating vs. Body Correlation: The rating and body have a higher correlation (0.2) than the other columns in the dataset. This suggests that the body of a wine may have some influence on its rating. Wines with a fuller body may receive higher ratings.


![download-1](https://user-images.githubusercontent.com/123442350/231897386-31ffecb2-bff1-498d-9897-d2b787f1b18a.png)


Best Model Metrics

The best model for this task is the Random Forest model with the following metrics:

Train MSE: 0.01, R2: 0.64
Test MSE: 0.01, R2: 0.46
Best parameters: {'model__max_depth': 6, 'model__n_estimators': 50}
Model Performance in Solving Business Problem
The Random Forest model performs reasonably well in predicting wine ratings. With an R2 score of 0.46 on the test set, it can explain 46% of the variance in the target variable. While not perfect, this model provides a reasonable starting point for predicting wine quality. Further refinements can improve the model's performance.

Summary and Recommendations

Based on the model performance and analytical findings, we provide the following recommendations for stakeholders:

Focus on wine body: As the body of a wine has a positive correlation with its rating, winemakers should pay attention to the body of their wines. Producing wines with a fuller body may lead to higher ratings and, consequently, increased sales.

Consider the price-quality relationship: The moderate correlation between price and rating suggests that higher-priced wines tend to have better ratings. Stakeholders should carefully consider their pricing strategies to balance profitability with perceived quality.

While the Random Forest model is a good starting point, we recommend exploring additional feature engineering techniques and other machine learning algorithms to improve the model's performance. This will enable stakeholders to make more accurate predictions and better informed decisions to improve their wine quality and sales.
