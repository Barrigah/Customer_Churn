# Customer_Churn
![customer churn](https://github.com/Barrigah/Customer_Churn/assets/141326495/5186d20e-a5a2-4fc9-aa05-cc4ed4974f3a)
<hr>
In this comprehensive project, we adopt an all-inclusive approach to predict customer churn by identifying specific criteria that indicate the likelihood of customers discontinuing their services.
<hr>

## Introduction
Customer churn, also referred to as customer attrition or customer defection, is a term used to describe the situation when customers terminate their association with a business or cease utilizing its products or services. It reflects the rate at which customers disengage or end their involvement with a company within a specific timeframe. The primary objective of this project was to predict potential churn customers using historical data provided by our client. It involved a classification problem that utilized a supervised machine learning approach. To begin the analysis, I formulated queries to join tables and extract the necessary data from the database. Through data exploration and transformation, and employing statistical techniques such as Variance Inflation Factor, Recursive Feature Elimination, and assessment of multicollinearity, I reduced the initial set of 158 derived features to the most crucial eight features. These selected features were utilized as the final set for prediction. The predictive model successfully identified over 4,000 potential churners, which has the potential to generate an additional annual revenue of over $2,000,000 for the business.
<hr>

## Problem Statement
The main challenge addressed in this Python-based project is to accurately forecast potential customer churn utilizing historical data, as supplied by our client
<hr>

## DATA SOURCING
The data originates from the Client Database, and dedicated code was developed to extract the requisite information for analysis. The database was seamlessly linked to a Python Jupyter Notebook using the Pandas and pyodbc libraries.

![Screenshot (107)](https://github.com/Barrigah/Customer_Churn/assets/141326495/25fa0550-f5dc-42b1-a743-7b4accda3d34)

<hr>

## Methodology

> The approach employed to address the problem encompassed several key steps, demonstrating a comprehensive methodology for churn prediction:

- Churn Definition: Churn was meticulously defined as the absence of any customer purchase within the last 8 months of business transactions, specifically, when the maximum or last transaction date is before October 31, 2007.

- Exploratory Analysis: An exploratory analysis was undertaken to gain insights into the characteristics of churners. This analysis involved delving into demographic, transactional, and attitudinal data. A decision tree was utilized to establish a rule set for describing these customers, and distribution plots were created to visualize demographic variables against the churn target.

- Feature Engineering with RFM: The feature engineering phase incorporated the Recency-Frequency-Monetary (RFM) analysis. This analysis facilitated the creation of attributes such as recency, frequency, and lifetime value for each customer. Subsequently, RFM variables or RFM Scores were employed to construct a clustering model using the K-means algorithm, an unsupervised technique. The optimal number of clusters was determined using the elbow method. The resulting cluster assignments were integrated into the modeling and scoring variables, with the churn variable as the target.

- Data Refinement and Integrity: To ensure data integrity, a single customer view was established, meaning that the final dataset featured a single customer's data per row, eliminating duplicates.

- Modeling Phases: The modeling phases encompassed a comprehensive series of steps, beginning with statistical testing to assess multi-collinearity and overfitting. Distributions were investigated, and any outliers, extreme values, or spurious entries were identified. Missing values were imputed where applicable. Feature selection was conducted to streamline the variables. Data was partitioned into training, testing, or validation sets, or cross-validation techniques were employed. Multiple models were developed, compared, and evaluated, culminating in the selection of the most promising model.

- Model Deployment and Validation: The selected champion model was deployed or scored on an unseen dataset, which had not been part of the model development phase. This procedure ensured that the model's performance was assessed in a real-world context, devoid of any potential bias introduced during training.

- Revalidation and Finalization: Prior to launching the primary marketing campaign, a final revalidation of the model was conducted. This step guaranteed that the model's effectiveness and reliability were verified, setting the stage for a successful campaign rollout.





