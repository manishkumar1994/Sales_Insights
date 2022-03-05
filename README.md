# Sales_Insights

## Data Analysis Using Power BI and Tableau

## Objective

In this project, the objective is to create dashboard which can be used to unlock sales insight that are not visible before for sales team for decision support and automate them to reduced manual time spent in data gathering

## Motivation
The motivation waA to understand more about the business analytics tools that are widely used in companies and also to get some hands-on experience with Power BI and Tableau.

•	The goal is to create an automated dashboard providing quick and latest sales insight to support data driven decision making.

## Observations

According to the report, we can see that the sales are declining and that it may be due to a variety of factors, including

> Product Quality
> Discount
> Identify which areas your product to be sale
> Every business growth will take some time to show profit based on Team Hardwork
> Covid can also be the major reason

• Easy to trace which customer is providing high-profit margin


## Conclusion

The dashboard will allow the sales team to make better decisions and stop manually gathering data to save 20% of the time and reinvest it in value-added activity



•	Data Analysis in MySQL, Data cleaning in Power query and created dashboard 

### Data Analysis Using SQL
1) To show all customer records
    SELECT * FROM customers;

2) To show total number of customers

    SELECT count(*) FROM customers;

3) To show transactions for Chennai market (market code for chennai is Mark001

     SELECT * FROM transactions where market_code='Mark001';

4) To show distrinct product codes that were sold in chennai

    SELECT distinct product_code FROM transactions where market_code='Mark001';

5)  To show transactions where currency is US dollars

     SELECT * from transactions where currency="USD"

6) To show transactions in 2020 join by date table

     SELECT transactions.*, date.* FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020;

7) To show total revenue in year 2020,

      SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and transactions.currency="INR\r" or transactions.currency="USD\r";

8) To show total revenue in year 2020, January Month,

      SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and and date.month_name="January" and (transactions.currency="INR\r" or transactions.currency="USD\r");

9) To show total revenue in year 2020 in Chennai

   SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and transactions.market_code="Mark001";
   
   ### Dashboard link for tableu
   https://prod-uk-a.online.tableau.com/#/site/projectsalesinsights/workbooks/113496/views
   
  ![image](https://user-images.githubusercontent.com/88727612/156886191-4fd12c90-b0e8-49d9-a68e-a066e273842b.png)
  
  ![image](https://user-images.githubusercontent.com/88727612/156886248-d8630568-8388-45f4-8050-c9b0cf0b4f2d.png)

   
   

 


