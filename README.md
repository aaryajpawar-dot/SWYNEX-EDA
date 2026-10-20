SWYNEX-EDA

Exploratory data analysis on the cleaned cafe sales dataset from Task 1, done as part of my data analytics internship at SWYNEX Technologies.

Dataset

The cleaned data has 9,501 rows and 8 columns, covering sales from [start date] to [end date].

| Column | Description |
|---|---|
| Transaction ID | Unique ID for each sale |
| Item | Product sold |
| Quantity | Units bought |
| Price Per Unit | Price of one unit |
| Total Spent | Quantity x Price Per Unit |
| Payment Method | Cash, Credit Card, Digital Wallet or Unknown |
| Location | In-Store, Takeaway or Unknown |
| Transaction Date | Date of the sale |

Analysis Steps

1. Loaded the cleaned data and converted Transaction Date to a date type
2. Checked shape, missing values, duplicates and date range
3. Calculated mean, median, standard deviation and skew for Quantity, Price Per Unit and Total Spent
4. Counted and compared Item, Payment Method and Location
5. Plotted monthly revenue, monthly orders and revenue by weekday
6. Compared revenue and units by item, and built an Item x Location heatmap
7. Checked correlations between the numeric columns
8. Found outliers in Total Spent with the IQR method
9. Found unusual days using z-scores on daily revenue
10. Checked that Total Spent equals Quantity x Price Per Unit

Key Insights

| # | Insight | Evidence |
|---|---|---|
| 1 | Revenue is highest in [month] and lowest in [month] | Monthly revenue chart |
| 2 | [Item] brings [x]% of revenue, and the top two items bring [y]% | Revenue by item chart |
| 3 | [Item] sells the most units, but [item] earns the most revenue | Units vs revenue chart |
| 4 | Average daily revenue is [x] on weekdays and [y] on weekends | Weekday chart |
| 5 | [Location] gives [x]% of revenue and [payment method] is the most used | Pie charts and heatmap |
| 6 | [x]% of payment methods and [y]% of locations are still Unknown | Data check in notebook |
| 7 | Large orders are outliers but they are real, since totals match Quantity x Price | Boxplot |

## Charts

![Monthly trend](charts/01_monthly_trend.png)
![Revenue and units by item](charts/03_item_revenue_units.png)
![Item and location heatmap](charts/05_item_location_heatmap.png)
![Outliers by item](charts/07_boxplot_item.png)

## Files

- `cleaned_data.csv`: cleaned dataset from Task 1
- `EDA.ipynb`: Python notebook with all the analysis code
- `charts/`: all saved charts

## Tools Used

- Python
- pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab

## Related

Task 1 (data cleaning): [link to your Task 1 repo]
