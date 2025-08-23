# W5L6: Revenue Pareto and Scatter Plot

## Glossary

1. **Pareto Principle (80/20 Rule)**: The idea that roughly 80% of effects come from 20% of causes; in business, often used to identify top contributors to sales or revenue.
2. **SKU (Stock Keeping Unit)**: A unique identifier for each distinct product and service that can be purchased.
3. **Revenue**: The total income generated from sales of goods or services.
4. **Volume**: The quantity of units sold.
5. **Average Price**: The mean price at which a product is sold, often used when prices vary.
6. **VLOOKUP**: An Excel function used to look up and retrieve data from a specific column in a table.
7. **Pivot Table**: A data summarization tool in Excel/Sheets used to sort, reorganize, group, count, total, or average data.
8. **Currency Formatting**: Displaying numbers as monetary values, often with commas and currency symbols.
9. **Cumulative Revenue**: The running total of revenue as you move through a list of items.
10. **Descending Order**: Sorting data from highest to lowest.
11. **Filter**: A tool to display only the rows in a table that meet certain criteria.
12. **Bar Chart**: A chart with rectangular bars representing data values.
13. **Line Chart**: A chart that displays information as a series of data points connected by straight lines.
14. **Scatter Plot**: A graph in which two variables are plotted along two axes, revealing any correlation.
15. **Outlier**: A data point that differs significantly from other observations.
16. **Data Label**: Text or values displayed on a chart to identify data points.
17. **Series (in Charts)**: A set of related data points plotted in a chart.
18. **X Axis / Y Axis**: The horizontal (X) and vertical (Y) lines on a chart.
19. **Extreme Value**: A value that is much higher or lower than most of the data.
20. **Annotation**: Notes or labels added to a chart for explanation or emphasis.

---

## Structured Notes

### Introduction

- The session explores how to analyze revenue and volume data using Pareto analysis and scatter plots in Excel.
- Focus is on identifying which SKUs contribute most to revenue and how to visualize this data.

### Calculating Revenue Using VLOOKUP

- Revenue requires both price and volume data.
- Price data is imported from the SKU master table using VLOOKUP in Excel.
- VLOOKUP is set up to match SKU names and retrieve the average price.
- Formula includes exact match (FALSE) and uses absolute references for the lookup range.
- Once price is added, revenue is calculated as: `Units Sold × Price per Unit`.
- Format revenue as currency for clarity.

### Summarizing Revenue with Pivot Tables

- Pivot tables are used to aggregate revenue by SKU across all cities and dates.
- Steps:
  - Select all relevant columns (A–F) from the sales data.
  - Insert a pivot table with SKUs as rows and sum of revenue as values.
  - Filter out blanks and sort SKUs by revenue in descending order.
  - Format revenue as currency for readability.
- Cumulative revenue is calculated to analyze the Pareto effect.
- Calculate percentage contribution of each SKU to total revenue.

### Pareto Analysis Results

- Top SKUs (e.g., one SKU contributing 25% of revenue) are identified.
- The 80/20 rule is observed: about 20% of SKUs contribute 80% of revenue.
- The tail (SKUs with little or no revenue) is discussed; these may be candidates for discontinuation.
- Comparison with volume data shows that high-revenue SKUs are not always high-volume SKUs.

### Visualizing Data: Bar, Line, and Pareto Charts

- Create charts to visualize revenue and cumulative percentage contribution.
- Use bar charts for revenue and line charts for cumulative percentage.
- Limit cumulative percentage to 100% for clarity.
- Compare volume and revenue Pareto charts to observe differences in distribution.

### Scatter Plot Analysis

- Combine revenue and volume data in a single pivot table.
- Use scatter plots to visualize the relationship between volume (X-axis) and revenue (Y-axis) for each SKU.
- Different product categories (e.g., FMCG, Lifestyle, Mobile) are plotted as separate series.
- Outliers (e.g., a single mobile SKU with very high revenue) can distort the chart; removing them can clarify patterns.
- Data labels are added to identify SKUs on the scatter plot.
- Removing outliers and certain categories (e.g., mobiles) can make the chart more interpretable.

### Key Insights

- Pareto analysis helps identify which products drive most of the revenue.
- Scatter plots reveal the relationship between sales volume and revenue, highlighting outliers and product category differences.
- Data visualization and filtering are essential for actionable business insights.

---

## Examples

- **VLOOKUP Formula Example:**
  - `=VLOOKUP(B2, 'SKU Master'!$B$1:$E$31, 4, FALSE)`
- **Pivot Table Setup:**
  - Rows: SKU
  - Values: Sum of Revenue, Sum of Volume
- **Pareto Chart:**
  - Bar: Revenue per SKU
  - Line: Cumulative % of Revenue
- **Scatter Plot:**
  - X-axis: Volume
  - Y-axis: Revenue
  - Series: Product categories (FMCG, Lifestyle, Mobile)

---

## Key Points

- Use VLOOKUP to merge price data into sales data for revenue calculation.
- Pivot tables and sorting help identify top-performing SKUs.
- Pareto analysis (80/20 rule) is useful for focusing on high-impact products.
- Scatter plots can reveal outliers and category differences in sales patterns.
- Data visualization aids in communicating insights to stakeholders.

### Metadata

- Title:W5L6_Revenue Pareto and Scatter Plot

- URL:<https://www.youtube.com/watch?v=HOfl_ESI78U>

### Notes

- ([00:00](https://www.youtube.com/watch?v=HOfl_ESI78U&t=0s)) ### Summary
The text discusses a detailed analysis involving sales and revenue data using Excel. It highlights the process of importing price data, calculating revenue, and creating pivot tables and charts to visualize sales performance. The use of functions like VLOOKUP is emphasized for automating data retrieval, while the importance of identifying revenue-generating SKUs (Stock Keeping Units) is stressed. The analysis reveals that a small percentage of SKUs contributes to a significant portion of total revenue, demonstrating a Pareto-like distribution. The text concludes with suggestions for further analysis and visualization to aid decision-making.

### Highlights

- **Automating Data Retrieval**: The text emphasizes the use of VLOOKUP in Excel to automate the extraction of price data from SKU Master to Sales Master.
- **Revenue Calculation**: It explains how revenue is calculated by multiplying units sold by price per unit.
- **Pivot Tables for Analysis**: The creation of pivot tables is discussed as a method to summarize revenue data across various dimensions such as SKU, city, and date.
- **Identifying Key Revenue Contributors**: The analysis identifies that a small number of SKUs contribute disproportionately to revenue, aligning with the 80/20 rule.
- **Visualization Techniques**: The text discusses creating scatter plots to visualize the relationship between sales volume and revenue, highlighting differences across categories.
- **Outlier Management**: It addresses the importance of removing outliers in charts to enhance clarity and presentation.
- **Recommendations for Action**: The narrative suggests that low-revenue, high-volume items should be reconsidered in inventory management.

### Key Insights

- **VLOOKUP Efficiency**: The use of the VLOOKUP function is crucial for efficiently merging price data with sales data, allowing for accurate revenue calculation without manual effort.
- **Revenue vs. Volume Dynamics**: The analysis shows that while some SKUs generate high revenue, others may sell in large volumes without contributing significantly to overall revenue, indicating a need for differentiated inventory strategies.
- **Pareto Principle Application**: The findings reflect the Pareto principle, where a small fraction of SKUs (20%) contributes to a large portion of revenue (80%), suggesting a focused approach on high-performing items.
- **Pivot Table Utility**: Pivot tables serve as a powerful tool for aggregating and visualizing data, enabling quick insights into revenue trends by SKU and other dimensions.
- **Importance of Data Visualization**: The text highlights the role of charts in presenting complex data simply and effectively, aiding stakeholders in understanding performance metrics.
- **Outlier Impact on Analysis**: The presence of outliers can skew visualizations, emphasizing the need for careful data cleaning before analysis.
- **Inventory Optimization**: Decisions about inventory should be guided by revenue contribution analysis, potentially leading to the discontinuation of low-performing SKUs.

### Outline

1. **Introduction**
   - Overview of the analysis context.
   - Importance of data-driven decision-making in sales.

2. **Data Importation**
   - Explanation of the need to merge pricing data from SKU Master to Sales Master.
   - Introduction to VLOOKUP as a tool for automation.

3. **Revenue Calculation**
   - Definition of revenue and its calculation method (units sold x price).
   - Manual vs. automated calculation processes.

4. **Using Pivot Tables**
   - Steps to create pivot tables for summarizing sales data.
   - Insights gained from analyzing revenue by SKU, city, and date.

5. **Revenue Distribution Analysis**
   - Discussion of the Pareto principle in the context of SKU revenue contributions.
   - Identification of high-revenue contributors versus low-revenue items.

6. **Data Visualization Techniques**
   - Importance of visualizing data using charts and pivot tables.
   - Steps to create scatter plots to compare volume and revenue.

7. **Outlier Management**
   - The effect of outliers on data interpretation.
   - Strategies for handling outliers in visualizations.

8. **Conclusion**
   - Summary of key findings and recommendations.
   - Emphasis on the need for continued analysis and adjustment in inventory strategy.

### Keywords

- VLOOKUP
- Revenue
- Pivot Table
- SKU (Stock Keeping Unit)
- Pareto Principle
- Data Visualization
- Outlier

### FAQs

- **Q1: What is VLOOKUP and how is it used?**
  - A1: VLOOKUP is an Excel function used to look up and retrieve data from a specific column in a table. It helps automate the process of merging data sets, such as prices from SKU Master to sales data.

- **Q2: How is revenue calculated in the analysis?**
  - A2: Revenue is calculated by multiplying the number of units sold by the average price per unit for each SKU.

- **Q3: What is the significance of pivot tables in sales analysis?**
  - A3: Pivot tables allow for the aggregation and summarization of large data sets, making it easier to analyze revenue trends across different dimensions like SKU and location.

- **Q4: What does the Pareto principle mean in the context of this analysis?**
  - A4: The Pareto principle, or 80/20 rule, suggests that a small percentage of SKUs (about 20%) contribute to a large portion of total revenue (around 80%), highlighting the need to focus on high-performing products.

- **Q5: Why is managing outliers important in data visualization?**
  - A5: Outliers can distort the overall picture in visualizations, making it difficult to interpret data correctly. Cleaning outlier data helps present a more accurate and clear analysis.

### Core Concepts

- **Data Integration**: The process of merging different data sources (like SKU pricing and sales data) is crucial for accurate analysis. Using Excel functions such as VLOOKUP facilitates this integration.
- **Revenue Understanding**: Revenue is a vital metric for assessing business performance, defined as the product of sales volume and unit price. Understanding how to calculate and analyze it can drive strategic decisions.
- **Pivot Tables**: These are powerful tools in Excel that allow users to summarize and analyze data efficiently. They help extract meaningful insights from large datasets by enabling users to view data from multiple perspectives.
- **Revenue Contribution Analysis**: Analyzing how different SKUs contribute to total revenue can inform inventory management and sales strategies, emphasizing high-value items.
- **Visualization**: Effective data visualization is essential for communicating findings. Charts like scatter plots can reveal relationships between variables, such as revenue and sales volume, aiding in understanding trends.
- **Outlier Identification**: Recognizing and managing outliers is critical in data analysis. Outliers can skew results and lead to misleading conclusions if not addressed properly.
- **Strategic Inventory Management**: The analysis underscores the need for strategic decision-making regarding inventory based on revenue contributions, focusing on retaining high-performing SKUs while reconsidering low-contributing items.

This response meets the specified requirements, maintaining clarity and coherence while providing a comprehensive analysis of the content.

-- With NoteGPT
