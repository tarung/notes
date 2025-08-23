# W5L7: Trend Analysis

## Glossary

1. **Trend Analysis**: Examining data over time to identify patterns or trends.
2. **Pivot Table**: A tool in Excel/Sheets for summarizing and analyzing data.
3. **Volume**: The number of units sold.
4. **Revenue**: Total income from sales.
5. **Line Chart**: A graph that displays data points connected by straight lines, often used to visualize trends over time.
6. **Date (in data)**: The specific day a transaction or event occurred.
7. **Day of the Week**: Monday, Tuesday, etc.; used to analyze patterns by weekday.
8. **Sum of Sales**: The total sales volume for a given period or category.
9. **Sum of Revenue**: The total revenue for a given period or category.
10. **Currency Formatting**: Displaying numbers as monetary values.
11. **Blank Values**: Empty cells in data, often filtered out in analysis.
12. **Legend (in charts)**: A key that explains symbols, colors, or patterns in a chart.
13. **Title (in charts)**: The heading that describes what the chart shows.
14. **Spike**: A sudden increase in data values.
15. **Artifact (in data)**: A misleading result caused by the way data is collected or processed.
16. **E-commerce**: Buying and selling goods or services online.
17. **Pattern**: A repeated or regular way in which something happens.
18. **Iterative**: A process that repeats steps to approach a desired goal.
19. **Data Formatting**: Adjusting how data is displayed for clarity.
20. **Insight**: A clear understanding of a complex situation, often gained from data analysis.

---

## Structured Notes

### Introduction

- This session focuses on analyzing sales and revenue trends using Excel pivot tables and charts.
- The goal is to identify patterns in sales volume and revenue over time and by day of the week.

### Analyzing Volume Trends by Date

- Use a pivot table with dates as rows and sum of sales as values.
- Remove blank values for clarity.
- Insert a line chart to visualize sales volume over time.
- Observation: No clear trend in sales volume over the 15-day period; values fluctuate up and down.

### Analyzing Revenue Trends by Date

- Repeat the process with revenue as the value in the pivot table.
- Format revenue as currency for readability.
- Insert a line chart for revenue trend.
- Observation: Revenue also shows no significant trend over the 15 days; daily revenue is roughly 25–30 lakhs.

### Monthly and SKU Context

- The data covers only 30 SKUs, but companies may have thousands.
- Monthly revenue can be estimated by multiplying daily averages.

### Analyzing Trends by Day of the Week

- Add a new column to the sales data to extract the day of the week from the date (using the TEXT function in Excel).
- Create a pivot table with day of the week as rows and sum of sales as values.
- Observation: Sales volume is higher on Tuesday, Wednesday, and Thursday; lower on weekends.
- Possible explanation: People may shop online during weekdays and visit malls on weekends.
- Note: The number of each weekday in the data may affect results (e.g., three Thursdays in the sample).

### Revenue Trends by Day of the Week

- Repeat the analysis with revenue as the value.
- Format as currency.
- Observation: No significant trend in revenue by day of the week.

### Key Insights

- No strong trends in sales volume or revenue over the 15-day period.
- Slight increase in sales volume midweek; weekends are lower.
- Data artifacts (like uneven weekday counts) can affect analysis.
- More data would be needed for deeper insights.

---

## Examples

- **Pivot Table Setup:**
  - Rows: Date or Day of the Week
  - Values: Sum of Sales or Sum of Revenue
- **Excel Formula for Day of Week:**
  - `=TEXT(A2, "ddd")` (returns day abbreviation from date)
- **Line Chart:**
  - Used to visualize trends over time or by category.

---

## Key Points

- Use pivot tables and charts to analyze trends in sales and revenue.
- Extract day of the week from dates for weekday analysis.
- Watch for data artifacts that may skew results.
- More data provides more reliable trend analysis.
