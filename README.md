# CavalierGroup_DTI_01_FinalProject
- ⭐[Ivan Robi Septian](https://github.com/Ivan-R-Septian), [Shafa Salzabila Meidita](https://github.com/shafameidita), [Ammar Muzaki Maftuh](https://github.com/Zacky182)
- 📊[Tableau Dashboard](https://public.tableau.com/app/profile/shafa.salzabila.meidita/viz/CAVAutoinsurance/CavalierDashboard)
- 📓[Notebook Analysis](https://github.com/PurwadhikaDev/CavalierGroup_DTI_01_FinalProject/blob/main/Autoinsurance_Cavalier.ipynb)
- 🔖[Customer Lifetime Value Dataset](https://www.kaggle.com/ranja7/vehicle-insurance-customer-data)

<p align="center">
  <img src="https://i.imgur.com/omRnugM.png" alt="logo" />
</p>
## Context
**CAV AutoInsurance**, a well-established auto insurance provider since 2000, operates in a highly competitive market. To sustain growth and improve its market position, the company aims to enhance its marketing strategies and customer retention efforts. Specifically, **CAV AutoInsurance** seeks to develop a more targeted approach to customer retention and optimize its marketing campaigns. By understanding the value of each customer, the company intends to allocate resources more effectively, maximize the impact of its campaigns, and ultimately drive better customer engagement and increased profitability.

## Business Problem Statement
In 2011, CAV AutoInsurance was confronted with a substantial obstacle, with only 14.6% of their insured customers electing to renew their policies following a retention campaign. This low renewal rate revealed that 85.4% of their customers were not engaged, indicating that their current strategy of treating all customers the same was both ineffective and resource-intensive. The broad, one-size-fits-all approach failed to address the diverse needs of their customer base, emphasising the necessity for a more targeted and efficient strategy to enhance customer retention and optimise marketing efforts.

1. The marketing team launched a new campaign, categorizing efforts based on the Months Since Policy Inception, dividing them into three equal segments. This campaign was structured into three tiers, each with different costs:
- Marketing Campaign Low: 539 customers (0-34 months) at $25 each.
- Marketing Campaign Medium: 513 customers (35-63 months) at $50 each.
- Marketing Campaign High: 509 customers (64-99 months) at $150 each.

2. CAV AutoInsurance is experiencing significant challenges in analyzing Customer Lifetime Value (CLV) and improving customer retention. The company currently faces an 85.4% customer churn rate, and recent marketing efforts, segmented by the number of month since policy inception <sup>[1](https://www.upwork.com/hire/data-analysts/cost/)</sup>, have not produced the expected results, leading to inefficient use of resources and low customer engagement. The current manual process for CLV analysis, which costs $20 per customer and takes approximately per hours, is both costly and time-consuming, limiting the company’s ability to scale its operations effectively.

The company recognised the need for a more advanced solution and engaged a data science team to develop a new strategy based on customer data. This strategy aims to predict and understand the value of each customer, creating a more targeted approach that will engage customers more effectively and improve retention by focusing on their specific needs.

Key Points:

1. What steps can we take to optimise our sales strategy in order to retain our customers?
2. How can machine learning models be developed to accurately predict Customer Lifetime Value (CLV)? This will enable us to understand customer value and make decisions regarding management strategies.
3. How can we develop a clustering model to effectively segment customers? This will help us to manage risk and improve customer engagement and retention.
4. How can we accurately predict customer behaviour and optimise marketing strategies across diverse customer segments? This will help us to maximise revenue and retention. We must identify the most impactful characteristic influencing customer decisions.

## Summary
#### **Best Performing Offer and Sales Channel**:
- Offer 2 with Agent Sales Channel shows the highest retention percentage of 28.01% with total 241 renewals. This indicates that customers are more likely to renew when presented with Offer 2 through agents. 

Improvement (%)= 
Average Retention Rate
Offer 2 Agent Retention Rate−Average Retention Rate
​
 ×100
  
The average retention rate across all other combinations is 9.99%. By using Offer 2 through Agent, which has a retention rate of 28.01%, we can see a potential improvement. However, realistically, this strategy could improve customer retention by around 40%, considering various practical factors that might limit the full potential of this approach. While the theoretical improvement suggests a much higher percentage, it's important to set achievable expectations based on real-world conditions.

#### **Optimizing Customer Lifetime Value**
The Random Forest model used to predict car insurance Customer Lifetime Value (CLV) showed exceptional accuracy, with a **Mean Absolute Percentage Error (MAPE)** of **3.3%** and an **adjusted R²** of **93%**. These results ensure that the company can make highly accurate estimates of customer value, significantly reducing the risk of over- or underestimating CLV.

Predicting CLV is critical to identifying the most valuable customers, allowing the company to effectively target its strategies and investments. By minimising errors in CLV predictions, the company can make informed financial decisions, optimise resource allocation and focus on customers with the highest potential value. This approach not only increases profitability, but also reduces the risk of underperforming investments, leading to more effective and strategic business outcomes.

#### **Customer Segmentation**
The insights from the Gold Cluster represents the highest-value customers with an average CLV of $13,277.98  demonstrate a number of actionable approaches to enhance customer satisfaction and retention for CAV AutoInsurance. The key strategies include enhancing premium coverage offerings, adjusting communication based on education levels, focusing on retired customers, strengthening engagement in suburban areas, and maximising the effectiveness of agent sales channels. Implementing these strategies will enable the company to better meet the needs of its Gold customers, ultimately leading to improved satisfaction and loyalty.

#### **Understanding with AI**
Explainable AI reveals that number of Policies and Monthly Premium Auto are the most impactful features across all clusters. In the Gold cluster, Number of Policies contributes up to +4,090.03 to the model’s predictions, while Monthly Premium Auto adds +2,185.60. These features are also significant in the Silver and Bronze clusters, though with slightly lower contributions: for Number of Policies, +1,934.88 in the Bronze cluster and +1,854.52 in the Silver cluster; for Monthly Premium Auto, +1,460.78 in the Silver cluster and +1,357.61 in the Bronze cluster.

Other features like Income and Employment Status further enhance predictions, particularly in the Gold segment, with contributions of +171.84 and +118.78, respectively. This analysis underscores the importance of suit strategies based on cluster-specific feature importance to optimize outcomes for different customer groups.

#### **Manual Customer Lifetime Value (CLV) Analysis**

Implementing the Random Forest model to automate Customer Lifetime Value (CLV) analysis offers a substantial financial advantage for the company. Conducting a manual CLV analysis for each customer involves significant costs, both in terms of time and resources. Each manual analysis incurs an expense of $20 and requires approximately 2 hours to complete, factoring in the time needed for reporting, communication, and other related tasks.

*Calculation*
- Cost per hour analysis: $20
- Amount of Data: 6,161 customers
- Estimation manual analysis per hour : 10 data (including analysis, reporting, and communication)

- Rate per Data Point:

Rate per Data Point = Price per hour / Data points per hour
Rate per Data Point = $20 / 10 = $2 per data point


- Total Payment:

Total Payment = Rate per Data Point × Number of Data Points
Total Payment = $2 × 6,161 = $12,322

*Calculate Total Weeks Required*

- Total Hours Required:

    - Total Hours Required = Number of Data Points / Data points per hour
    - Total Hours Required = 6,161 / 10 = 616.1 hours

- Total Weeks:

    - Total Weeks = Total Hours Required / Hours per Week
    - Total Weeks = 616.1 / 40 ≈ 15.4 weeks

Total Payment: $12,322
<br>
Total Weeks Required: 15.4 weeks


Given the total dataset of 6,161 customers, the manual process would require an estimated total payment of $12,322 and approximately 616.1 hours of work. With a standard workweek of 40 hours, this equates to about 15.4 weeks of full-time work.


*Cost Savings*

If a Data Scientist using Machine Learning charges $6,000 for a month-project<sup>[2](https://www.interviewquery.com/p/data-science-consultant-salary)</sup>, the cost savings for the company would be the difference between the manual analysis cost ($12,322) and the automated process cost using the Data Scientist's services.

Cost Savings: $12,322 - $6,000 = *$6,322*

*Time Savings*

By using a Data Scientist who can finish the project in 4 weeks, the company saves:
15.4 weeks (manual analysis) - 4 weeks (Data Scientist) = *11.4 weeks*

*Percentage Time Saved*:

$$
\text{Percentage Time Saved} = \left(\frac{\text{Manual Time} - \text{Automated Time}}{\text{Manual Time}} \right) \times 100
$$


$$
\text{Percentage Time Saved} = \left(\frac{15.4 \text{ weeks} - 4 \text{ weeks}}{15.4 \text{ weeks}} \right) \times 100 \approx 74.03\%
$$


So, the company can save approximately *74.03%* of the time by using a Data Scientist for the CLV analysis.

<br>Thus, the company can save $6,322 in costs and reduce the project timeline by 11.4 weeks (74.03%) by using a Data Scientist for the analysis.

#### **Marketing Campaign**
In 2011, CAV AutoInsurance faced a significant challenge with an alarming 85.4% customer churn rate. In response, the marketing team launched a new campaign, categorizing efforts based on the Months Since Policy Inception, dividing them into three equal segments. This campaign was structured into three tiers, each with different costs:

- Marketing Campaign Low: 539 customers (0-34 months) at $25 each.
- Marketing Campaign Medium: 513 customers (35-63 months) at $50 each.
- Marketing Campaign High: 509 customers (64-99 months) at $150 each.

Total Marketing Campaign Cost: $124,775

While this approach was straightforward, it lacked a strategic method for accurately determining the value of each insurance customer. To address this, the data science team utilized machine learning to predict Customer Lifetime Value (CLV), providing insights into the true worth of each customer to the company. Furthermore, machine learning was employed to create customer clusters, enabling more targeted and cost-effective marketing campaigns.

**Cost Savings Calculation**

Using machine learning-driven clusters, the campaign costs were recalculated:

- Bronze Campaign: 872 customers x $25 = $21,800
- Silver Campaign: 550 customers x $50 = $27,500
- Gold Campaign: 184 customers x $150 = $27,600

Total Marketing Campaign Cost: $76,900

Cost Savings: $47,875

**Segmentation Analysis**

Without machine learning, the average CLV for each campaign category was:

Campaign Category

- Marketing Campaign High: $6,768.73
- Marketing Campaign Medium: $6,456.90
- Marketing Campaign Low: $6,805.53

With machine learning, the average CLV for each cluster was:

Cluster

- Gold: $13,760.27
- Silver: $8,698.53
- Bronze: $4,015.14

The machine learning approach provided a more accurate representation of customer value, revealing significant differences across clusters, as opposed to the traditional categories, which showed incorrect CLV order.

By leveraging machine learning, CAV AutoInsurance not only achieved more accurate customer segmentation but also optimized its marketing spend. This advanced approach led to smarter resource allocation, potentially saving the company substantial amounts of money and effort by targeting the right customers with the right offers. This resulted in a total cost savings of $47,875.


## Recommendation
**Model Recommendations**:
- Ensure a comprehensive data dictionary is in place, so that all features used in the model are well-defined and not based on assumptions. This will prevent misunderstandings and ensure consistency in data interpretation.
- Verify that there are no data entry errors during dataset collection, particularly in critical features like Income, Months Since Policy Inception, and Months Since Last Claim.
- Incorporate additional features, such as Customer Satisfaction and Retention Rate, to better assess customer loyalty.
- Expand the dataset, especially above $16,484 price range, to enhance the model's predictive accuracy.
- Improve the model's predictive performance through parameter tuning, using the current benchmarks as a reference point for optimization.
- Explore using DBScan clustering for customer segmentation. This method is more robust to outliers and can handle larger datasets, which may improve segmentation quality.

**Business Recommendations**:
- Enhance Offer2 Agents Channel Reach Across Other Offer Type:
    - Offer2 is particularly successful in driving renewals via the Agent channel. CAV AutoInsurance should explore ways to replicate this success in other Offers. Suit the offer presentation or providing special incentives in these channels could help increase renewals by 40%. 
    - Expand Digital Outreach for Web and Call Center Channels, Web and Call Center channels show moderate engagement, their renewal rates lag behind. CAV AutoInsurance could improve digital communication strategies, such as personalized email campaigns or online customer support, to boost customer confidence in renewing policies through these channels.

- Combine the CLV prediction model with clustering segmentation to optimize customer targeting in marketing campaigns. Aim for a 20% increase in conversion rates over the next 1 years by identifying and segmenting high-value customers. Tailor marketing messages to the specific needs of these segments, which will improve customer acquisition and retention, especially in the Gold insurance segment.

- Enhance customer service by creating a dedicated support team for Gold customers. Introduce regular engagement initiatives to increase customer satisfaction by 20% and reduce churn by 7.5% within the next year. Provide specialized training to support staff and implement engagement tools like personalized communications and loyalty programs to build stronger relationships.

- Increase the Number of Policies in the Gold cluster to leverage its significant impact on customer retention, targeting a 15% improvement in retention rates. Optimize Monthly Premium Auto to enhance overall customer lifetime value (CLV), aiming for a 10-15% uplift across all clusters. Additionally, use insights from Income and Employment Status to tailor marketing strategies, with the goal of boosting engagement rates by approximately 10%. Implementing these strategies can lead to improved profitability and a stronger competitive advantage.

- Invest in utilizing a Data Scientist to automate Customer Lifetime Value (CLV) analysis through machine learning. By implementing this approach, the company can achieve significant cost savings of $6,322 compared to manual analysis and reduce the project timeline by 11.4 weeks, resulting in approximately 74.03% time savings. This strategic shift not only enhances operational efficiency but also allows the organization to reallocate resources toward more strategic initiatives, ultimately driving greater value and insights from the CLV analysis.

- Permanently implement machine learning for customer segmentation and CLV prediction because it can significantly reduce marketing costs by 38.4%, achieved through more efficient resource allocation and precise targeting of customers. This approach not only optimizes the use of marketing budgets but also enhances the effectiveness of campaigns, ensuring that resources are directed towards the most valuable customer segments. By leveraging machine learning, the company can make data-driven decisions that maximize both cost efficiency and marketing impact, leading to improved overall business performance.

- Develop an application based on the created model to streamline predictions and segmentation, supporting CAV Autoinsurance's operational goals.
