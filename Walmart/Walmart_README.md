Walmart Sales Data: Comprehensive Analysis and Strategic Decision-Making Report







Executive Summary
This analysis of Walmart's weekly sales data from 2010-2012 reveals critical insights into seasonal trends, store performance, and the impact of external economic factors. Key findings include significant sales spikes during holiday periods, a strong negative correlation between unemployment and sales, and the ability to segment stores into three distinct performance clusters. The data provides a robust foundation for strategic decisions in inventory management, marketing, store operations, and financial forecasting. Implementing the recommended actions will optimize operations and drive revenue growth.









1. Data Overview and Preparation
The dataset is clean and well-structured, providing a solid foundation for analysis.

Code:

<img width="292" height="184" alt="image" src="https://github.com/user-attachments/assets/e09b65a9-edd9-4ca3-bef0-d80a81f04702" />




Output:

<img width="292" height="168" alt="image" src="https://github.com/user-attachments/assets/30bdccde-4d98-45f8-949d-69be3ec6fdaf" />

 



The data contains 6,435 records across 8 variables with no missing values or duplicates, ensuring the integrity of our analysis.

Code:

<img width="257" height="176" alt="image" src="https://github.com/user-attachments/assets/396cb982-2fe8-4c51-ad76-3b5118f01a60" />
 




Output:

<img width="257" height="193" alt="image" src="https://github.com/user-attachments/assets/52ce3461-0452-4fe2-a86c-387f383908e3" />




 
2. Strategic Planning & Financial Forecasting
Question: Based on the clear seasonal trends and quarterly patterns, how should we set our annual sales targets and allocate our budget for inventory and marketing across different quarters?
Analysis: We analyzed sales trends by month and quarter to identify seasonal patterns.

Code:

<img width="252" height="174" alt="image" src="https://github.com/user-attachments/assets/9d3bfbca-f4f1-40b4-9d79-0d103a9985bc" />
 



Diagram:

<img width="468" height="206" alt="image" src="https://github.com/user-attachments/assets/2da40846-3742-404c-a7e9-868d5244f8c4" />




 
Findings & Recommendations:
•	Q4 is Dominant: Sales in Q4 are consistently ~ 60% higher than in other quarters due to the holiday season (Thanksgiving, Christmas).
•	Steady Growth: Average sales show a slight year-over-year increase from 2010 to 2012 in Q1-Q3.
•	2012 Q4 Anomaly: 2012 Q4 sales were significantly lower than previous years; this warrants investigation into potential data or external factors.
Informed Decisions:
1.	Budget Allocation: Allocate 40-50% of the annual marketing and inventory budget to Q4 to capitalize on high demand.
2.	Inventory Planning: Work with suppliers to ensure stock levels are built up in late Q3 to meet Q4 demand.
3.	Target Setting: Set aggressive but achievable sales targets for Q4, while aiming for steady, incremental growth in Q1-Q3 based on the previous year's performance.

3. Store Operations & Performance Management
Question: Which stores are the top and bottom performers, and why is there such a significant variation?
Analysis: We ranked stores by total sales and analyzed their distributions.

Code:

<img width="311" height="172" alt="image" src="https://github.com/user-attachments/assets/da6f4813-3265-472c-b33d-d2d3d120a23a" />




 
Output:

<img width="180" height="100" alt="image" src="https://github.com/user-attachments/assets/c5565692-61ad-44a1-8c06-f19fb588a8af" />




 
Diagram:

<img width="404" height="216" alt="image" src="https://github.com/user-attachments/assets/a803e721-5d9d-40cf-afef-3801d766b281" />




 


<img width="404" height="182" alt="image" src="https://github.com/user-attachments/assets/52170979-01b9-4b19-8285-6ab580972f85" />




 
Findings & Recommendations:
•	Significant Disparity: Store 20 is the top performer, with sales nearly double that of the lowest-performing stores.
•	Consistency: Some stores have high variance (whiskers on the boxplot are long), indicating inconsistent performance, while others are stable.
Informed Decisions:
1.	Benchmarking: Launch a project to identify best practices from Store #20, #4, and #14 (e.g., layout, local marketing tactics, staffing models) and implement them in lower-performing stores.
2.	Root Cause Analysis: Mandate a deep-dive analysis into the bottom 5 performing stores to determine causes: is it location, local competition, poor management, or store size?
3.	Performance Incentives: Tie store manager bonuses to both total sales and consistency (reducing variance), encouraging stable performance.

4. Marketing & Promotions
Question: Holidays have a statistically significant impact on sales. Which specific holidays drive the largest sales lifts?
Analysis: We compared sales on holiday vs. non-holiday weeks and measured the impact by month.

Code:

<img width="261" height="156" alt="image" src="https://github.com/user-attachments/assets/031d573f-5a24-4fff-a914-458f0a7016b5" />




 
Output:

<img width="260" height="163" alt="image" src="https://github.com/user-attachments/assets/dfba4b45-f920-4722-b7c2-9f812ae8fa17" />




 
•	Major Impact: Holiday weeks see ~24% higher sales on average than non-holiday weeks. The p-value of 0.0000 confirms this is not random.
•	Top Holidays: December (Christmas) and November (Thanksgiving) have the most significant impact by far.
Informed Decisions:
1.	Campaign Focus: Concentrate the most prominent marketing campaigns (TV, digital ads, circulars) around November and December.
2.	Promotional Planning: Plan "doorbuster" deals and major promotions for the weeks leading up to Thanksgiving and Christmas to capture the full wave of demand.
3.	Budget justification: Use the 24% sales lift metric to justify increased marketing spend during all holiday periods, not just year-end.

5. Economic Strategy & Risk Management
Question: How do external factors like Unemployment and CPI affect our sales?
Analysis: We calculated the correlation of external factors with Weekly Sales.

Code:
 
<img width="236" height="159" alt="image" src="https://github.com/user-attachments/assets/1ebe432b-7653-4331-94c8-4e268257bd47" />





Output:

<img width="171" height="91" alt="image" src="https://github.com/user-attachments/assets/028f46a9-465d-4aa9-b385-465e81840c22" />
 




Diagram:

<img width="236" height="202" alt="image" src="https://github.com/user-attachments/assets/0d0a6249-cf62-4151-afcc-097c7b7815fa" />




 
Diagram:

<img width="416" height="177" alt="image" src="https://github.com/user-attachments/assets/0d17c5e8-a1bf-4dff-90c5-76fa72141d58" />




 
Diagram:

<img width="416" height="188" alt="image" src="https://github.com/user-attachments/assets/b2ac4817-213a-4849-99a2-0c8619cf9b07" />




 
Findings & Recommendations:
•	Unemployment: Has a moderate negative correlation (-0.20) with sales. As unemployment rises, sales tend to fall.
•	CPI (Consumer Price Index): Has a moderate positive correlation (0.19). This may indicate that as the general cost of living rises, more people shop at Walmart for its value proposition.
•	Weak Influences: Temperature and Fuel Price have almost no linear correlation with weekly sales.
Informed Decisions:
1.	Recession Planning: Develop a contingency plan for economic downturns. This should include a focus on promoting essential goods and value brands to retain cost-conscious customers.
2.	Market Positioning: Leverage the positive CPI correlation in marketing messaging: "Walmart helps you fight inflation."
3.	Ignore Noise: Do not base pricing or promotion strategies on fluctuations in fuel prices, as there is no measurable impact on sales.


6. Time Series Analysis of Weekly Sales
Question: How did the weekly sales fluctuate over the year?

Analysis: The analysis reveals fundamental characteristic of Walmart's sales data:
Clear and Predictable Seasonal Patterns:
•	The decomposition shows strong, recurring yearly seasonality (period=52 weeks). This is visually evident as large, consistent peaks that occur at the same point each year (corresponding to the year-end holiday season around November/December) and troughs (e.g., in January).
•	The trend component is relatively stable or slightly increasing over the 2010-2012 period. There is no evidence of a sharp decline or explosive growth, indicating a steady business operation.
•	The residuals (the noise left after removing trend and seasonality) appear random. This means the additive model effectively captured the major patterns, and there are no obvious, unexplained events distorting the data.

Code:

<img width="240" height="131" alt="image" src="https://github.com/user-attachments/assets/8b95bef8-dadb-4415-86e4-7824d517f38b" />




 
Diagram:
 
<img width="318" height="136" alt="image" src="https://github.com/user-attachments/assets/b183c30b-89e3-42c8-9fcd-3a68947ddc8d" />





Output:
 
<img width="134" height="58" alt="image" src="https://github.com/user-attachments/assets/87dc45f9-edc9-4e4b-9537-e6903a4b333a" />





7. Store Clustering for Targeted Strategies
Question: Based on the K-means clustering, what are the profiles of the three distinct store clusters?
Analysis: We grouped stores into clusters based on their sales and economic characteristics.

Code:
 
<img width="333" height="224" alt="image" src="https://github.com/user-attachments/assets/f06613c6-47d2-4697-a6a7-cd81d8a3cf7a" />





Output:

<img width="212" height="98" alt="image" src="https://github.com/user-attachments/assets/24188403-46ba-43b7-8a0b-f66049750ff4" />




 
Diagram:

<img width="387" height="168" alt="image" src="https://github.com/user-attachments/assets/7a3697e9-e909-4da3-9435-db72b009023c" />




 
Output:

<img width="226" height="116" alt="image" src="https://github.com/user-attachments/assets/20a8c892-8548-40b4-8892-a838b5f90eb6" />




 
Findings & Recommendations:
•	Cluster 2 (High Performers): 16 stores with the highest sales and lowest unemployment. Affluent, high-volume locations.
•	Cluster 0 (Average Performers): 18 stores with mid-level sales and economic indicators.
•	Cluster 1 (Low Performers): 11 stores with the lowest sales and highest unemployment. Struggling economic areas.
Informed Decisions:
1	Cluster-Specific Strategies:
	Cluster 2: Test new, premium products here first. Focus on customer experience and loyalty.
	Cluster 0: Implement best practices from Cluster 2 to drive growth. Focus on competitive pricing.
	Cluster 1: Optimize for value. Focus on essential goods and promote deep discounts. Assess the long-term viability of stores in severely economically depressed areas.
2.	Resource Allocation: Direct top managerial talent and renovation budgets to Cluster 2 and high-potential Cluster 0 stores to maximize ROI.


Summary: 

<img width="411" height="124" alt="image" src="https://github.com/user-attachments/assets/0e2e2d3b-f71e-49d0-b4de-764e073921ff" />





<img width="236" height="103" alt="image" src="https://github.com/user-attachments/assets/44db8214-6af9-471c-ae33-7dfc2289a50d" />



