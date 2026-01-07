# DAX Measures
## Total Sales
Calculates total chocolate sales revenue
```DAX
Total Sales Amount = SUM(Sales[Amount])
```
## Distinct product sold
```DAX
Distinct Products Sold = DISTINCTCOUNT(Sales[Product])
```
## Average order size by Region
```DAX
Average Order Size per Region = AVERAGEX(VALUES(sales[Boxes]), Sales[Boxes])
```
## Gross profit
```DAX
Gross Profit = [Total Sales Amount] - [Total Cost of Products Sold]
```
## Month-to-Date Sales
```DAX
Month-to-Date Sales = TOTALMTD([Total Sales Amount], 'Calendar'[Date])
```
## Salesperson Performance Score
```DAX
Salesperson Performance Score = [Total Boxes Sold]
```
## Profit Margin
```DAX
Profit Margin = DIVIDE([Gross Profit], [Total Sales Amount])
```
## Total Boxes Sold
```DAX
Total Boxes Sold = SUM(Sales[Boxes])
```
## Year-to-Date Sales
```DAX
Year-to-Date Sales = TOTALYTD([Total Sales Amount], 'Calendar'[Date])
```
## Average Sales per day
``` DAX
Average Sales per Day = AVERAGEX(VALUES('Calendar'[Date]), [Total Sales Amount])
```
## Total cost of product Sold
```DAX
Total Cost of Products Sold = SUMX(Sales, Sales[Boxes] * RELATED(products[Cost per box])
```
## Average Revenue Per Salesperson
```DAX
Average Revenue per Salesperson = AVERAGEX(VALUES(people[Sales person]), [Total Sales Amount])
```
