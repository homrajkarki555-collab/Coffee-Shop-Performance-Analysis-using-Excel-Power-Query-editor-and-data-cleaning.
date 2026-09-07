# Coffee-Shop-Performance-Analysis-using-Excel-Power-Query-editor-and-data-cleaning.
Developed an excel dashboard, that shows the performance of a coffee shop. This dashboard highlights the highest selling product and sales based on days, hours, weeks and months. 

## Data Source
This data is taken from an online website call <a href="https://mavenanalytics.io/data-playground?page=3&pageSize=5"> mavenanalytics.io </a>. You can tab on <a href= "https://mavenanalytics.io/data-playground/coffee-shop-sales?page=3&pageSize=5"> Download link </a>to Download the raw data from the source.

## Data Set
This point gives you the raw excel dataset. You can click the link to download/view the dataset.
- <a href= "https://github.com/homrajkarki555-collab/Coffee-Shop-Performance-Analysis-using-Excel-Power-Query-editor-and-data-cleaning./blob/main/Coffee%20Shop%20Sales.xlsx"> Raw excel dataset </a>

## Objective
The main objective of this project is to analyze retail sales data to gain actionable insights that will enhance the performance of the Coffee Shop.

### Recommended Analysis
- How do sales vary by day of the week and hour of the day?
- Are there any peak times for sales activity?
- What is the total sales revenue for each month?
- How do sales vary across different store locations?
- what is the average price/order per person
- Which products are the bestselling in terms of quantity and revenue?
- How do sales vary by product category and type?

## Skills Used
Excel, Pivot Table, Dashboard on Excel, Measures, Data cleaning on Power query editor. 

## Column Description
This points contains all the meta information regarding the columns described in the CSV files.
- transaction - Unique ID of the transaction made by the customer 
- transaction_date - Date of the transaction 
- transacttion_time - Time of the transaction 
- store_id- Unique ID of all stores 
- store_location - Location where the store is located 
- transaction_qty - Quantity of the product ordered 
- unit_price - Unit price of the product
- product_category - Category pf the product 
- product_type - type of the product
- product_detail - detail description of the product with size

## Custom created Columns 
This point contains all the custom columns created using the above given data columns 
- Custom - Size of the order as described in product_detail column, Sl for small, Mm for medium and Lg for large. 
- Total_bill - Total bill of the customer. Multiplied unit_price with transaction_qty to get total bill
- Month Name - Shows which month the transaction was made. Used month to get month name.
- Day Name - Shows which day the transaction was made. Used day of week to get day name 
- Hour - Shows which hour of the day the transaction was made. used transition_time to get hours of transaction. 
- Day of Week - Shows which day of week the transaction was made. Used transition_date to get day number
- Month - Shows which month the transaction was made. Used transition_date to get month number 

## Measures
- Average order - =sum(Transactions[transaction_qty])/DISTINCTCOUNT(Transactions[transaction_id])
- Footfall - =DISTINCTCOUNT(Transactions[transaction_id])
- total sales - =sum([Total_bill])
- Average Bill - =SUM(Transactions[Total_bill])/COUNT(Transactions[transaction_id])

## Strategic Business Insights


## SS Dashboard/ Excel workbook with dynamic dashboard 
- <a href="https://github.com/homrajkarki555-collab/Coffee-Shop-Performance-Analysis-using-Excel-Power-Query-editor-and-data-cleaning./blob/main/Screenshot%202026-09-06%20095521.png"> Dashboard Screenshot </a>
- <a href="https://github.com/homrajkarki555-collab/Coffee-Shop-Performance-Analysis-using-Excel-Power-Query-editor-and-data-cleaning./blob/main/Book1.xlsx"> Excel workbook with dynamic dashboard  </a>

## Decision



## Business Impact



## Author and Contact
- Homraj karki
- Data Analysis
- Email- homrajkarki555@gmail.com
- Linkdin- <a href="https://www.linkedin.com/in/homraj-karki/">Linkdin Profile </a>

