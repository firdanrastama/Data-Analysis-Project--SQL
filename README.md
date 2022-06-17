# Data Analysis Project using PostgreSQL

## Project Overview
This repository contains an exploratory data analysis on E-Commerce Public Dataset by Olist. In this project we want to explore the data to identify and analysis the sales performance at Olist Brazil and generate insights.

## Dataset
The dataset has information of 100k orders from 2016 to 2018 made at multiple marketplaces in Brazil. Its features allows viewing an order from multiple dimensions: from order status, price, payment and freight performance to customer location, product attributes and finally reviews written by customers. We also released a geolocation dataset that relates Brazilian zip codes to lat/lng coordinates. This is real commercial data, it has been anonymised, and references to the companies and partners in the review text have been replaced with the names of Game of Thrones great houses

Link for the dataset: [Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

Link for the PostgreSQL script: [SQL Script](https://github.com/firdanrastama/Data-Analysis-Project--SQL/blob/main/sql_script)

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
# Exploratory Data Analysis
## 1. Sales Performance by Year
This dataset contains orders information from 2016 to 2018. Let's see if there is an increase in sales from 2016 to 2018

![image](https://user-images.githubusercontent.com/80149518/174345661-a27f14ab-14c3-4238-ad74-9aab0d8c3eb4.png)


We can see in the figure that from 2016 to 2017 there is an increase on sales by 121% and from 2017 to 2018 there is a increase on sales by 20%. Since 121% is a massive increase we will try to investigate sales performance in 2016 and 2017. Let's investigate on monthly sales

![This is an image](https://github.com/firdanrastama/Data-Analysis-Project--SQL/blob/main/images/monthly_sales_2016_2017.png)

Based on the figure, we see that for 2016 we only have 3 months data recorded in database, and we have full months recorded in 2017. Hence we got a massive increase sales from 2016 to 2017

## 2. Customers Transactions per Year
After analyzed on sales performance, let's see the number of our customers transactions per year

![This is an image](https://github.com/firdanrastama/Data-Analysis-Project--SQL/blob/main/images/transactions_per_year.png)

Since we have only 3 months data in 2016, it does make sense that we only have 267 total number of transactions. Furthermore for 2017 to 2018 we have an increase of number of transactions by 21%

## 3. Customers Transactions per Month from 2016 to 2018

![This is an image](https://github.com/firdanrastama/Data-Analysis-Project--SQL/blob/main/images/transactions_per_month.png)

August is the highest number of transactions. How about the revenue? Is our best month by revenue also August? Let's investigate our total revenue per month from 2016 to 2018

## 4. Revenue per Month from 2016 to 2018

![This is an image](https://github.com/firdanrastama/Data-Analysis-Project--SQL/blob/main/images/revenue.png)

Based on the figure we can see that May is the most highest revenue from 2017 to 2018 *not include 2016 since only has 3 months data*. Since May is the most highest revenue, let's see what are the most items that our customers ordered in May

## 5. Top 15 Items Sold in May from 2017 to 2018

![This is an image](https://github.com/firdanrastama/Data-Analysis-Project--SQL/blob/main/images/may_items_orders.png)

## 6. Revenue per Week in May 2017 and May 2018

![This is an image](https://github.com/firdanrastama/Data-Analysis-Project--SQL/blob/main/images/revenue_per_week_may_2017.png)    ![This is an image](https://github.com/firdanrastama/Data-Analysis-Project--SQL/blob/main/images/revenue_per_week_may_2018.png) 

## 7. Customer Acquisition per Month

![image](https://github.com/firdanrastama/Data-Analysis-Project--SQL/blob/main/images/customer_acquisition.png)

Our highest customer acquisition is in November 2017 with 7544 new customers. In August 2018 we have 6512 new customers, however in the next month our customers acquisitions decreasing to only 16 new customers

## 8. Total Customers Over the Year
![image](https://user-images.githubusercontent.com/80149518/174141649-232be810-d15b-4f1e-bfa9-0aab86ad5701.png)

## 9. Growth Customers
![image](https://github.com/firdanrastama/Data-Analysis-Project--SQL/blob/main/images/growth_customers.png?raw=true)


## 10. Top 5 Total Customers per City
The success of business depends upon how well you understand your customers. Let's analyze our majority customers from

![This is an image](https://github.com/firdanrastama/Data-Analysis-Project--SQL/blob/main/images/city_customers.png)

Our biggest customers are from Sao Paulo. And our top 5 list cities are also one of the largest cities in Brazil. And the capital city Brasilia in 4th place on the list of our total customers.

## 11. Best City by Revenue Each Year
![image](https://user-images.githubusercontent.com/80149518/174266285-2918b81d-4919-40c8-abd2-f5c263ce3e2a.png)

Since our customers are mostly from Sao Paulo, It does make sense that Sao Paulo has the highest revenue compare to another cities in Brazil

## 12. Delivery Success Rate by Year
![image](https://user-images.githubusercontent.com/80149518/174269596-de1dc0bf-d09c-4087-ab2c-105dd9cbfc54.png)

In 2016 there was total 5 orders that did not delivered, with delivery failure rate only 2% and delivery success rate 98%. In 2017 100% orders are delivered to the customers, and in 2018 there was only 1 order that did not delivered

## 13. Customer Satisfication - Perfect Rating
![image](https://user-images.githubusercontent.com/80149518/174270879-77985079-b282-4fa4-92f0-245add143d1b.png)

- In 2016 customers that given a perfect rating up to 57%
- In 2017 customers that given a perfecet rating up to 60%
- In 2018 ustomers that given a perfecet rating up to 59%

There is an increase number by 1% from 2016 to 2017 and decreasing number from 2017 to 2018 by 1%
