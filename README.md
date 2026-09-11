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

## Business Insights
#### How do sales vary by day of the week and hour of the day?
- Our daily sales is in upward movement, with an average daily sales of $3860.80. Whereas we see a high number of sales in the morning between 7am to 10am and as the days continues the sales decreases which show that people usually prefers drinking tea/coffee early in the morning.   
#### Are there any peak times for sales activity?
- Between 7am to 10am are the peak time as the highest number of sales in the days happens during this time of the day. 
#### What is the total sales revenue for each month?
- The total sales revenue of each month are :-
<img width="251" height="145" alt="image" src="https://github.com/user-attachments/assets/455af369-b2db-46ba-8c7e-3ad2fd5ed38f" />

#### How do sales vary across different store locations?
- There are no huge difference in total sales and transaction count in between different sales location. Each store location gives as average total sales of $2,32,937.44.
<img width="466" height="97" alt="image" src="https://github.com/user-attachments/assets/d2d4c976-b325-4526-9939-0e0b7b10a1a2" />

#### what is the average price/order per person
- Average price per order is $4.69 and Average order per person is 1.4.
  
#### Which products are the bestselling in terms of quantity and revenue?
- The bestselling in terms of Quantity and revenue is Coffee. Total 89250 was sold which along contributes 39% of total quantity sold, giving the revenue of $2,69,952.45 

#### How do sales vary by product category and type?
- Coffee & Tea collectively generate $466,358.40, representing 66.7% of total business revenue and 74.1% of unit volume. In the Coffee category, Barista Espresso ($91,406.20) and Gourmet brewed coffee ($70,034.60) contribute roughly 60% of all coffee sales. In the Tea category, Brewed Chai tea dominates both volume (26,250 units) and revenue ($77,081.95), outperforming the other three tea varieties combined.

<img width="550" height="961" alt="image" src="https://github.com/user-attachments/assets/657f6488-c96c-4bf1-8e89-cbbc522d419e" />


## SS Dashboard/ Excel workbook with dynamic dashboard 
- <a href="https://github.com/homrajkarki555-collab/Coffee-Shop-Performance-Analysis-using-Excel-Power-Query-editor-and-data-cleaning./blob/main/Screenshot%202026-09-06%20095521.png"> Dashboard Screenshot </a>
- <a href="Coffee Shop Excel Table and Dasboard.xlsx"> Excel workbook with dynamic dashboard  </a>

## Decision
- Currently, our peak business occurs in the morning, leaving substantial untapped potential in the afternoon. We need an afternoon-specific campaign to drive traffic. For example, a 1:00 PM–4:00 PM 'Happy Hour' with special pricing on iced coffees and teas. This approach will attract the post-lunch crowd and lift sales during our slowest window of the day.
- The average transaction is just $4.69 — a strong sign most visits are single-item (one coffee, one tea) with little add-on selling. Bakery (scones, pastries, biscotti) makes up only about 12% of revenue even though foot traffic is huge — it's riding along on drink sales rather than being actively sold. A simple combo prompt such as ("add a scone for $X") or a coffee+pastry bundle priced slightly below buying separately could meaningfully raise the average ticket without needing a single new customer through the door.

## Business Impact
- 
- Currently the average transaction is per person is just $4.69. If we adopt the above method of combo prompts we can expect an  revenue increase by up to  10%. We have an transaction count of 149116 even if 10% of this people purchase the combo pack that we can  the average order per person will be £7. Our total revenue will grow from $698812.33 to $768245.63 that is an increase of $69433.30. That makes a jump of 10% in our revenue 


## Author and Contact
- Homraj karki
- Data Analysis
- Email- homrajkarki555@gmail.com
- Linkdin- <a href="https://www.linkedin.com/in/homraj-karki/">Linkdin Profile </a>

