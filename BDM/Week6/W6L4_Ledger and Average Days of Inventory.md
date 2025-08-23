# W6L4: Ledger and Average Days of Inventory

## Glossary

1. **Inventory**: The stock of goods held for sale or production.
2. **Stock**: The quantity of items available in storage.
3. **Go-down/Depot**: Warehouse or storage location.
4. **Sales Data**: Records of items sold over time.
5. **Opening Stock**: Inventory available at the start of a period.
6. **Pivot Table**: Excel tool for summarizing and analyzing data.
7. **SKU (Stock Keeping Unit)**: Unique identifier for each product.
8. **Filter (in Pivot Table)**: Used to focus on specific data, such as a single SKU.
9. **VLOOKUP**: Excel function to look up and retrieve data from a table.
10. **Cumulative Sales**: Running total of sales over time.
11. **Average Daily Sales**: Mean number of units sold per day.
12. **Days of Inventory Available**: Number of days current stock will last at average sales rate.
13. **Ledger**: Record of all inventory movements (inflows and outflows).
14. **Inward Stock**: Inventory received into storage.
15. **Outflow**: Inventory sold or removed from storage.
16. **Closing Stock**: Inventory remaining at the end of a period.
17. **Negative Stock**: When calculated stock goes below zero (should be avoided in practice).
18. **Reconciliation**: Ensuring records match actual stock.
19. **Stock Transfer**: Movement of inventory between locations.
20. **Excel Sheet**: Spreadsheet used for calculations and record-keeping.

---

## Structured Notes

### Introduction

- This session covers inventory management, focusing on whether there is enough stock to meet sales.
- Uses Excel to analyze stock levels, sales, and calculate days of inventory available.

### Calculating Days of Inventory Available

- Use the "open stock" sheet to find starting inventory for each SKU across cities.
- Calculate total opening stock (sum across cities).
- To estimate how long stock will last:
  - Find average daily sales for the SKU (using sales data and pivot tables).
  - Divide opening stock by average daily sales.
  - Example: If opening stock is 272 units and average daily sales is 28.6, then days of inventory = 272 / 28.6 ≈ 9.5 days.
- This method assumes sales rates remain constant.

### Using Pivot Tables and Filters

- Create a pivot table with date as rows and volume as values, filtered for a single SKU.
- Use VLOOKUP to fetch opening stock for the selected SKU.
- Change the filter to analyze different SKUs.

### Cumulative Sales and Stock Depletion

- Calculate cumulative sales to see when stock will run out.
- Compare opening stock to cumulative sales to estimate the last day stock is available.
- This is a forward-looking estimate; actual sales may vary.

### Handling Inward Stock and Transfers

- For locations like Madras, consider both sales (outflow) and inward stock (transfers from other locations).
- Calculate daily closing stock: Opening stock - Sales + Inward stock.
- Use a ledger sheet to track daily movements and reconcile stock.
- Ensure closing stock never goes negative; set to zero if needed.

### Practical Excel Tips

- Use pivot tables for daily outflow by city and SKU.
- Use VLOOKUP for fetching opening stock and sales data.
- Maintain a ledger for each location to track opening stock, sales, inward stock, and closing stock.
- Reconcile records daily to ensure accuracy.

### Key Insights

- Days of inventory available is a key metric for stock management.
- Combining sales, stock, and inward transfers gives a complete picture of inventory health.
- Excel tools like pivot tables, filters, and VLOOKUP simplify inventory analysis.
- Regular reconciliation prevents errors and negative stock situations.

---

## Examples

- **Days of Inventory Formula:**
  - `Days of Inventory = Opening Stock / Average Daily Sales`
- **Ledger Columns:**
  - Date, Opening Stock, Sales, Inward Stock, Closing Stock
- **Pivot Table Setup:**
  - Rows: Date
  - Values: Volume (filtered by SKU and city)
- **VLOOKUP Example:**
  - `=VLOOKUP(B1, 'Open Stock'!$A$1:$E$31, 5, FALSE)`

---

## Key Points

- Use average daily sales to estimate how long stock will last.
- Track inventory movements with a ledger for each location.
- Use Excel tools for efficient inventory analysis and reconciliation.
- Prevent negative stock by regular checks and accurate record-keeping.

### Metadata

- Title:W6L4_ Ledger and Average Days of Inventory

- URL:<https://www.youtube.com/watch?v=D3ShGOyQ58A>

### Notes

- ([00:00](https://www.youtube.com/watch?v=D3ShGOyQ58A&t=0s)) ### Summary
The discussion revolves around inventory management, specifically analyzing stock levels to ensure adequate supply for ongoing sales. The team emphasizes the importance of understanding opening stock across different cities and calculating how long that stock will last based on daily sales. They explore creating pivot tables to analyze sales data and utilize functions like VLOOKUP to track inventory. The conversation highlights the need for accurate forecasting and understanding stock movements over time to prevent stockouts and manage inventory effectively.

### Highlights

- The importance of having sufficient inventory to fulfill sales needs.
- Use of pivot tables to analyze daily sales and inventory levels.
- Calculation of how long the current stock will last based on average daily sales.
- Discussion of stock movements, including incoming and outgoing stock.
- The relevance of maintaining a ledger to track daily inventory changes.
- The necessity of considering historical sales data for more accurate forecasting.
- Visualization of inventory data through charts for better analysis and understanding.

### Key Insights

- **Inventory Sufficiency**: The discussion emphasizes that having enough inventory on hand is crucial for fulfilling customer orders. Inventory shortages can lead to missed sales opportunities.
  
- **Data Analysis Tools**: The use of pivot tables and VLOOKUP in Excel illustrates how data analysis tools can assist in inventory management by providing clear insights into stock levels and sales trends.

- **Forecasting Sales Duration**: By dividing the opening stock by the average daily sales, the team can estimate how many days the current stock will last, which is crucial for planning reorder levels.

- **Stock Movement Tracking**: Understanding the inflow and outflow of stock is vital for maintaining optimal inventory levels. A ledger system is suggested to help monitor daily changes in inventory.

- **Historical Data Utilization**: The importance of considering past sales data for accurate forecasting is highlighted, as it can provide a more reliable basis for estimating future sales trends.

- **Adjusting for Growth**: The conversation touches on the need to adjust inventory calculations based on expected growth in sales, indicating that static averages may not always be sufficient.

- **Visualization for Better Decision-Making**: Creating charts to visualize inventory data allows for easier interpretation and can aid in discussions about inventory management strategies.

### Outline

1. **Introduction to Inventory Management**
   - Importance of inventory in sales fulfillment
   - Overview of key challenges in managing inventory

2. **Analyzing Opening Stock**
   - Calculation of total opening stock across cities
   - Importance of knowing stock levels at warehouse openings

3. **Sales Data Analysis**
   - Using pivot tables to analyze daily sales
   - VLOOKUP for tracking stock levels

4. **Estimating Stock Longevity**
   - Calculating how many days stock will last based on average daily sales
   - Importance of accuracy in forecasting stock duration

5. **Stock Movements and Ledger Maintenance**
   - Tracking incoming and outgoing stock to manage inventory levels
   - The role of a ledger in recording daily stock changes

6. **Historical Data for Forecasting**
   - Utilizing past sales data to improve inventory forecasts
   - Adjusting predictions based on growth trends

7. **Data Visualization Techniques**
   - Creating charts to represent inventory and sales data
   - Importance of visual tools in decision-making processes

8. **Conclusion**
   - Summary of best practices in inventory management
   - Future considerations for continuous improvement in stock handling

### Keywords

- Inventory Management
- Stock Levels
- Sales Data
- Pivot Tables
- VLOOKUP
- Forecasting
- Data Visualization

### FAQs

- **Q1: Why is inventory management important for sales?**
  - A1: Effective inventory management ensures that sufficient stock is available to meet customer demand, preventing lost sales opportunities.

- **Q2: What tools can be used for analyzing inventory data?**
  - A2: Tools like Excel pivot tables and functions such as VLOOKUP can be used to analyze sales and inventory data effectively.

- **Q3: How can businesses estimate how long their stock will last?**
  - A3: By dividing the opening stock by the average daily sales, businesses can estimate the number of days their current stock will last.

- **Q4: What is the purpose of maintaining a ledger in inventory management?**
  - A4: A ledger helps track the daily inflow and outflow of stock, providing insights into inventory changes over time.

- **Q5: How does historical sales data impact inventory forecasting?**
  - A5: Historical sales data can help businesses make more accurate predictions about future sales trends, allowing for better inventory planning.

### Core Concepts

- **Inventory Sufficiency**: Maintaining adequate stock levels is crucial for meeting sales demands.
- **Data Analysis**: Utilizing analytical tools like pivot tables aids in understanding inventory dynamics.
- **Stock Longevity Calculation**: Estimating how long stock will last based on sales data helps in making informed decisions about reordering.
- **Movement Tracking**: Monitoring stock movements (inflows and outflows) is vital for effective inventory management.
- **Historical Data Importance**: Leveraging past sales data enhances forecasting accuracy.
- **Growth Adjustments**: Adjusting inventory strategies based on expected sales growth is essential for maintaining balance.
- **Visualization**: Using charts for data representation facilitates better understanding and decision-making in inventory management.

### Length

This response contains a total of 1,020 words.

-- With NoteGPT
