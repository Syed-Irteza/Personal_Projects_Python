Walmart Sales Data: Comprehensive Analysis and Strategic Decision-Making Report























Executive Summary
This analysis of Walmart's weekly sales data from 2010-2012 reveals critical insights into seasonal trends, store performance, and the impact of external economic factors. Key findings include significant sales spikes during holiday periods, a strong negative correlation between unemployment and sales, and the ability to segment stores into three distinct performance clusters. The data provides a robust foundation for strategic decisions in inventory management, marketing, store operations, and financial forecasting. Implementing the recommended actions will optimize operations and drive revenue growth.




















1. Data Overview and Preparation
The dataset is clean and well-structured, providing a solid foundation for analysis.
Code:
  
Output:
 

The data contains 6,435 records across 8 variables with no missing values or duplicates, ensuring the integrity of our analysis.
Code:
 
<img width="186" height="138" alt="image" src="https://github.com/user-attachments/assets/7015982d-1a5a-4ef8-a62d-ea7bd349d046" />


Output:
 
2. Strategic Planning & Financial Forecasting
Question: Based on the clear seasonal trends and quarterly patterns, how should we set our annual sales targets and allocate our budget for inventory and marketing across different quarters?
Analysis: We analyzed sales trends by month and quarter to identify seasonal patterns.
Code:
 









Diagram:
 
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
 
Output:
 
Diagram:
 
Diagram:
 
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
 
Output:
 
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
 

Output:
 

Diagram:
 
Diagram:
 
Diagram:
 
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
 
Diagram:
 

Output:
 


7. Store Clustering for Targeted Strategies
Question: Based on the K-means clustering, what are the profiles of the three distinct store clusters?
Analysis: We grouped stores into clusters based on their sales and economic characteristics.
Code:
 


Output:
 
Diagram:
 
Output:
 
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

<img width="468" height="612" alt="image" src="https://github.com/user-attachments/assets/b420059e-a730-405e-917c-91d9de040859" />
