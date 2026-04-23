# Supermarket Visualizations

A collection of data visualizations built in R for exploring a supermarket sales dataset (`supermarket.csv`).

## Dataset

The script reads from `supermarket.csv` and uses the following columns:

| Column | Description |
|---|---|
| `unit_cost` | Cost per unit of a product |
| `items_count` | Number of items in an order |
| `satisfaction_score` | Customer satisfaction rating |
| `department` | Store department (e.g., Electronics) |
| `city_branch` | City/branch where the sale occurred |
| `delivery_time` | Delivery time in minutes |

## Visualizations

The script produces 9 individual plots and one combined dashboard view:

1. **Scatter Plot – Unit Cost vs Satisfaction Score**  
   Plots unit cost on the x-axis against satisfaction score on the y-axis to explore any relationship between price and customer satisfaction.

2. **Bar Chart – Total Items Count by Department**  
   Shows the total number of items sold, grouped by department.

3. **Pie Chart – Electronics Sales by City Branch**  
   Displays the share of electronics sales across different city branches as percentages.

4. **Box Plot – Unit Cost Distribution**  
   Summarises the spread and outliers of unit cost values across all orders.

5. **Histogram – Satisfaction Score Distribution**  
   Shows the frequency distribution of customer satisfaction scores.

6. **Dot Chart – Average Satisfaction Score by Department**  
   Compares the mean satisfaction score across all departments.

7. **Bar Chart – High Delivery Time Orders by Department**  
   Counts orders with a delivery time of 90 minutes or more, broken down by department.

8. **Density Plot – Satisfaction Score**  
   A smoothed density curve of the satisfaction score distribution.

9. **Pairs Plot – Delivery Time, Satisfaction Score, Unit Cost**  
   A pairwise scatter plot matrix showing relationships between the three numeric variables.

10. **Combined Dashboard (2×4 Grid)**  
    Plots 1–8 displayed together in a single 2-row by 4-column layout for a quick overview.

## Requirements

- R (any recent version)
- Base R graphics (no additional packages required)

## Usage

1. Place `supermarket.csv` in the same working directory as `visualizations.R`.
2. Open R or RStudio and run:

```r
source("visualizations.R")
```

All plots will be rendered sequentially. The final output is the combined 2×4 dashboard showing plots 1–8 side by side.
