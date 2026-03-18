📊 Project Overview

This project provides a comprehensive analysis of retail sales and inventory management. By leveraging a targeted subset of the "Retail Sales Dataset" from Kaggle, I performed data cleaning, feature engineering, and statistical modeling entirely within Excel to uncover key insights into sales patterns, pricing strategies, and stock efficiency.

🛠️ Data Preparation & Methodology
•	Data Selection: A representative sample of the first 500 records was curated and structured for deep-dive analysis.
•	Feature Engineering: I enhanced the dataset by developing two critical business metrics:
o	Stock Efficiency: (Units Sold / Inventory Level) Evaluates how effectively inventory is converted into revenue.
o	Price Difference: (Company Price - Competitor Pricing) Identifies the company's competitive market positioning.

📈 Detailed Pivot Table Analysis & Findings
I prepared 6 specialized Pivot Tables to answer specific business questions. Each analysis is supported by dedicated charts:
1.	Sales by Product Category:
o	Objective: Identify which categories generate the highest sales volume.
o	Finding: Toys emerged as the top-performing category.
2.	Sales Performance by Region:
o	Objective: Analyze geographic sales distribution.
o	Finding: The West region leads with the highest sales volume.
3.	Seasonal Demand Analysis:
o	Objective: Examine the impact of seasonality on product demand.
o	Finding: Demand peaks in Spring, while Autumn shows the lowest performance.
4.	Average Price by Product Category:
o	Objective: Understand category-level pricing strategies.
o	Finding: Clothing has the highest average price, while Groceries is the lowest.
5.	Inventory Efficiency Analysis:
o	Objective: Evaluate how efficiently inventory is utilized (Stock Turnover).
o	Finding: Clothing is the most efficient category in terms of inventory turnover.
6.	Competitive Pricing Analysis:
o	Objective: Compare company prices against market rivals.
o	Finding: Prices in Electronics and Toys are higher than competitors (positive values), while other categories maintain a price leadership (negative values).

🚀 Key Performance Indicators (KPIs)
The dashboard features dynamic KPIs for an immediate business snapshot, calculated using formulas:
•	Top Performing Category: Dynamically identified using:
=INDEX(Sheet3!B65:B69, MATCH(MAX(Sheet3!C65:C69), Sheet3!C65:C69, 0))
•	Global Metrics: Total Sales, Average Unit Price, and overall Efficiency were calculated using SUM and AVERAGE functions.

🖥️ Interactive Dashboard
Retail Sales & Inventory Insights Dashboard was designed with:
•	Visuals: Sales by Category, Pricing Competitiveness, Regional Distribution, and Inventory Efficiency.
•	Interactivity: Integrated Slicers for Region and Category for granular, real-time data filtering.

🔬 Statistical Modeling & Predictive Insights
To elevate the project from descriptive to predictive analytics, I performed a Simple Linear Regression analysis to model the relationship between inventory value and demand forecast.
Model Specification
•	Dependent Variable (Y): Inventory Value (Calculated as Inventory Level * Unit Price).
•	Independent Variable (X): Demand Forecast.
Regression Results & Technical Interpretation
The model yielded high statistical significance, providing a data-driven foundation for inventory budgeting:
1.	Correlation & Explanatory Power:
o	Multiple R (0.40): Indicates a moderate positive correlation. As demand forecasts rise, inventory investment tends to increase accordingly.
o	R Square (0.16): The model explains approximately 16% of the variance in inventory value. While this might seem low in a controlled environment, in a retail context, it highlights that inventory levels are influenced by a complex mix of factors beyond just forecasts—such as warehouse capacity, lead times, and promotional cycles.
2.	Statistical Reliability:
o	Significance F ($1.13 \times 10^{-20}$): This value is near zero, proving that the relationship between these variables is highly statistically significant and not due to random chance.
3.	Predictive Coefficient:
o	Demand Forecast Coefficient (38.93): For every 1-unit increase in the demand forecast, the total inventory value is expected to increase by an average of 38.93 units. This coefficient serves as a baseline for future stock procurement planning.
The regression analysis confirms a statistically significant link between forecasted demand and inventory investment ($p < 0.05$). The residual variance (the 84% not explained by the model) reflects critical operational constraints such as physical storage limits, supplier-mandated Minimum Order Quantities (MOQ), and safety stock buffers maintained against supply chain volatility.

