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
