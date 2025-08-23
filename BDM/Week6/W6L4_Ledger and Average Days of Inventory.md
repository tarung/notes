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
