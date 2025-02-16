# Pizza Sales Analysis Dashboard

#### Dashboard Link: https://drive.google.com/drive/folders/1gTvaJosJPumJ0uN-J1CeiIyomjJHywOm?usp=sharing

This dashboard will help the organization to understand their sales better from different perspectives. It will help the organization to know about their total sales, average sales, and number of items sold. This dashboard will also help them know about the top 5 best and bottom 5 worst-selling products.

### Problem Statement

#### KPI Requirements:
1.	Total Sales – The sum of the total price of all pizza orders.
2.	Average Order Value – The average amount spent per order, calculated by dividing the total sales by the total number of orders.
3.	Total Pizzas Sold – The sum of quantities sold.
4.	Total Orders – The total number of orders placed.
5.	Average Pizzas Per Order – The average number of pizzas sold per order, is calculated by dividing the total number of pizzas sold by the total number of orders.


#### Charts Requirements:
1.	Daily trend for total orders – Create a bar chart that displays the daily trend of total orders over a specific time period. This chart will help us identify any patterns or fluctuations in order volumes daily.
2.	Hourly trend for Total Orders – Create a line chart that illustrates the hourly trend of total orders throughout the day. This chart will allow us to identify peak hours or periods of high-order activity.
3.	Percentage of Sales by Pizza Category – Create a pie chart that shows the distribution of sales across different pizza categories. This chart will provide insights into the popularity of various pizza categories and their contribution to overall sales.
4.	Percentage of Sales by Pizza Size – Generate a pie chart that represents the percentage of sales attribute to different pizza sizes. This chart will help us understand customer preferences for pizza sizes and their impact on sales.
5.	Total Pizzas Sold by Pizza Category – Create a funnel chart that presents the total number of pizzas sold for each pizza category. This chart will allow us to compare the sales performance of different pizza categories.
6.	Top 5 Best Sellers by Total Pizzas Sold – Create a bar chart highlighting the top 5 best-selling pizzas based on the total number of pizzas sold. This chart will help us identify the most popular pizza options.
7.	Bottom 5 Worst Sellers by Total Pizzas Sold – Create a bar chart showcasing the bottom 5 worst-selling pizzas based on the total number of pizzas sold. This chart will enable us to identify underperforming or less popular pizza options.

### Steps followed

#### - Data Connection
       Dataset was connected to MS Excel through SSMS
#### - Data Cleaning
       Changed the pizza_size values S -> Regular, M -> Medium, L -> Large, XL -> X-Large, XXL -> XX-Large
#### - Data Processing
       1. Build a new column "order_day" that shows only the day according to the date column "order_date". The function used to extract the name of the day from the particular date was: =TEXT([@[ORDER_DATE]], "dddd"
       2. As the instances of order_id attribute are repetitive and there is no Distinct Count function in the pivot table, a custom function was developed to find the total unique orders from repetitive order_id. The function is: 1/COUNTIF(B:B,[@[order_id]])
#### - Data Analysis
#### - Dashboard Building

### Insights
A single page report was generated in MS Excel
![Image](https://github.com/user-attachments/assets/7c91a44a-aa63-4187-96f4-bdd6b1329481)
