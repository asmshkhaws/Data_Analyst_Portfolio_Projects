A. KPI’s
--1. Total Revenue:
--2. Average Order Value
--3. Total Pizzas Sold
--4. Total Orders
--5. Average Pizzas Per Order
--------------------------------------------------------------------------------------------------------------------
B. Daily Trend for Total Orders
--------------------------------------------------------------------------------------------------------------------
C. Hourly Trend for Orders
--------------------------------------------------------------------------------------------------------------------
D. % of Sales by Pizza Category for January Month
--------------------------------------------------------------------------------------------------------------------
E. % of Sales by Pizza Size
--------------------------------------------------------------------------------------------------------------------
F. Total Pizzas Sold by Pizza Category
--------------------------------------------------------------------------------------------------------------------
G. Top 5 Best Sellers by Total Pizzas Sold
--------------------------------------------------------------------------------------------------------------------
H. Bottom 5 Best Sellers by Total Pizzas Sold
---------------------------------------------------------------------------------------------------------------------
--NOTE:
--If you want to apply the Month, Quarter, Week filters to the above queries you can use WHERE clause. Follow some of below examples
--SELECT DATENAME(DW, order_date) AS order_day, COUNT(DISTINCT order_id) AS total_orders 
--FROM pizza_sales
--WHERE MONTH(order_date) = 1
--GROUP BY DATENAME(DW, order_date)

--*Here MONTH(order_date) = 1 indicates that the output is for the month of January. MONTH(order_date) = 4 indicates output for Month of April.

--SELECT DATENAME(DW, order_date) AS order_day, COUNT(DISTINCT order_id) AS total_orders 
--FROM pizza_sales
--WHERE DATEPART(QUARTER, order_date) = 1
--GROUP BY DATENAME(DW, order_date)

--*Here DATEPART(QUARTER, order_date) = 1 indicates that the output is for the Quarter 1. MONTH(order_date) = 3 indicates output for Quarter 3.
