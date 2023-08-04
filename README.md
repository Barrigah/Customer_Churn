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

<hr>

## Commercial Impact of our churner prediction.

Evaluating the commercial impact of our churner prediction holds significant importance. By proactively identifying customers who are likely to churn, we can strategize and implement targeted retention efforts. This approach has the potential to lead to substantial benefits, including:

Revenue Preservation: Pinpointing potential churners allows us to focus resources on retaining high-value customers, thereby safeguarding revenue streams that might otherwise be lost.

Cost Savings: Instead of expending resources on broad retention campaigns, we can tailor our interventions specifically to the identified churners. This targeted approach can result in cost savings while maximizing effectiveness.

Customer Loyalty Enhancement: Addressing the needs and concerns of customers on the verge of churning demonstrates a commitment to their satisfaction. Successfully retaining these customers can foster long-term loyalty and positive word-of-mouth referrals.

Data-Driven Decision Making: Our churner prediction model equips us with actionable insights derived from data analysis. This empowers decision-makers to make informed choices about resource allocation, marketing strategies, and customer engagement.

Optimized Marketing Efforts: By understanding the characteristics and behaviors of potential churners, we can tailor marketing campaigns and offers to resonate more effectively with these segments.

Competitive Advantage: Proactively managing customer churn can set us apart from competitors who might be less adept at identifying and retaining at-risk customers.

Long-Term Growth: The cumulative effect of successful churn reduction over time can contribute to sustainable business growth and improved financial performance.

In conclusion, the commercial impact of our churner prediction lies in its potential to drive revenue retention, cost efficiency, customer loyalty, and strategic decision-making. It positions our company for enhanced competitiveness and sustained growth in a dynamic market landscape.

<hr>

## Commercial Impact
A total of 6,464 customers were assessed and scored. Among them, 572 customers are predicted to be inclined towards churn, while a significant majority of 5,837 customers are expected to remain loyal. On average, each customer generates an annual revenue of £1,975. Anticipating the potential success of our churning prevention strategy, the estimated commercial value amounts to $1,129,897.00.
 
 ![image](https://github.com/Barrigah/Customer_Churn/assets/141326495/d12b3163-cfdf-439c-9c38-4464e7ca9aab)

<hr>

## Recommendations to Prevent Churn:

- Proactive Identification and Targeted Interventions: Implement a weekly assessment to identify customers who haven't made purchases in the last 5 months. These customers should be categorized as potential churners. Upon identifying such customers, initiate immediate targeted retention efforts.

- Personalized Offers: Upon identifying potential churners, promptly send them personalized promotional vouchers or discount coupons. These incentives can rekindle their interest, showcasing a commitment to their satisfaction and encouraging continued engagement.

- Leverage Recommendation Model: Utilize our recommendation model to suggest relevant products to potential churners. By tailoring promotions to align with their preferences, we can increase the likelihood of re-engagement and purchases.

- Solicit Feedback and Input: Actively engage with potential churners by seeking their feedback and recommendations on product offerings and specifications. This engagement not only demonstrates a genuine interest in their preferences but also encourages them to become active participants in our product improvement process.


<hr>

## By implementing these recommendations, we can foster the following positive outcomes:

>- Retention: The personalized offers and promotions will entice potential churners to make purchases, reducing the likelihood of churn and preserving valuable revenue streams.

>- Cost Efficiency: Targeted interventions ensure that resources are channeled effectively, avoiding unnecessary expenses on broad campaigns. This approach optimizes cost savings while enhancing results.

>- Loyalty and Advocacy: Addressing potential churners' needs showcases a commitment to their satisfaction, fostering long-term loyalty. Successful retention efforts can transform them into brand advocates, contributing to positive word-of-mouth referrals.

>- Data-Informed Actions: The churner prediction model and engagement feedback provide us with actionable insights. These insights guide informed decisions on resource allocation, marketing strategies, and customer interactions.

>- Enhanced Competitiveness: Proactively managing churn demonstrates our proactive stance in comparison to competitors. This approach sets us apart by showcasing our ability to identify and retain at-risk customers effectively.

>- Sustained Growth: Over time, successful churn reduction efforts contribute to sustainable business growth and improved financial performance. The cumulative effect reinforces our position in the market landscape.

>- By following these strategies, we position ourselves to not only prevent churn but also enhance customer loyalty, drive revenue retention, and ensure sustained growth in the ever-evolving market dynamics.


















