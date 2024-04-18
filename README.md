# Sales-Insights-Tableau

Link to the dashboard: https://prod-useast-a.online.tableau.com/t/tableaumahesh/views/Sales_Insights/Dashboard1

### Preview

<img width="1503" alt="image" src="https://user-images.githubusercontent.com/59694546/220733586-afb9bb5a-a436-4c50-95df-d48b010b83b2.png">


## Project Objective and Success Criteria (AIMS Grid)

<img width="1661" alt="image" src="https://user-images.githubusercontent.com/59694546/220734774-7c75281f-af42-422b-bb7f-9e5475cbc331.png">


### Data Analysis Using SQL

1. Show all customer records

    `SELECT * FROM customers;`

1. Show total number of customers

    `SELECT count(*) FROM customers;`

1. Show transactions for Chennai market (market code for chennai is Mark001

    `SELECT * FROM transactions where market_code='Mark001';`

1. Show distrinct product codes that were sold in chennai

    `SELECT distinct product_code FROM transactions where market_code='Mark001';`

1. Show transactions where currency is US dollars

    `SELECT * from transactions where currency="USD"`

1. Show transactions in 2020 join by date table

    `SELECT transactions.*, date.* FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020;`

1. Show total revenue in year 2020,

    `SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and transactions.currency="INR\r" or transactions.currency="USD\r";`
	

Credit : Codebasics
