# Pizza-Shop-Sales-Analysis
# 1. Projact Name:- Pizza shop sales analysis using Power Bi

# 2. Introduction:-
The Pizza Shop Sales Analysis project is a comprehensive business intelligence report built using Power BI, designed to provide actionable insights into the sales performance of a pizza shop. By analyzing historical order data, this project aims to uncover key trends in customer preferences, product performance, and revenue generation. With the help of interactive visualizations and calculated metrics, stakeholders can make data-driven decisions to optimize operations, enhance customer satisfaction, and increase profitability. The analysis leverages various Power BI features such as DAX, KPIs, slicers, and dynamic dashboards to present a clear and compelling picture of the pizza shop’s business activity.

# 3. Project Objective:-
The primary objective of the Pizza Shop Sales Analysis project is to leverage Power BI to extract valuable business insights from historical pizza order data. The aim is to support data-driven decision-making by providing a clear view of sales performance, customer preferences, and product trends. Specific objectives include:
       1. To analyze total revenue and quantity sold over various time periods (daily, monthly, hourly).
       2. To identify the best-selling pizzas based on quantity and revenue.
       3. To evaluate sales distribution across different pizza sizes and categories.
       4. To monitor average order value and overall order trends.
       5. To present insights through interactive visualizations and KPIs for easy interpretation by business stakeholders.

# 4. Project Overview:-
The Pizza Shop Sales Analysis project was developed using Power BI to explore and analyze structured pizza sales data. The dataset provided was clean, well-structured, and in a flat table format, eliminating the need for data cleaning or relational modeling. The focus was on building effective measures, KPIs, and visual dashboards to extract and present business insights. Here’s a step-by-step breakdown of how the project was carried out:

        1. Data Loading with Power Query:
              A. The dataset was directly imported into Power BI using Power Query.
              B. Since the data was already clean, minimal transformation was needed.
              C. Data types were auto-detected and verified.

        2. Transformation (Minimal):
              A. Basic steps like column renaming and creation of helper columns (e.g., Year, Month, Day from order_date) were done for better analysis.
         
        3.DAX Measures:
          Several DAX measures were created to compute business metrics, including:
               A. Total Revenue
               B. Total Orders
               C. Total Quantity Sold
               D. Average Order Value
               E. Daily, Monthly, and Hourly Sales

        4. KPIs (Key Performance Indicators):
           Visual KPIs were built to highlight critical metrics at a glance:
               A. Total Revenue
               B. Total Pizzas Sold
               C. Average Revenue per Order
               D. Best-Selling Pizza

        5. Visualizations:
           A variety of charts were used to bring insights to life:

           A. Bar Chart – for top-selling pizzas and sales by pizza size.
           B. Column Chart – to show monthly and hourly sales trends.
           C. Funnel Chart – to represent category-wise or size-wise quantity breakdown.
           D. Area Chart – to track revenue over time.
           E. Pie Chart – for category and size distribution.

        6. Dashboard Design:
           An interactive and user-friendly dashboard was designed with filters and slicers to analyze performance across 
           different dimensions like time, pizza size, and category.

# 5. Project Dataset:
The dataset used in this project contains historical order data from a pizza shop. It is structured as a flat table with each row representing an individual pizza order. The dataset includes key information such as order details, product type, pricing, quantity, and timestamps. The columns in the dataset are:
 
       1. order_id – Unique identifier for each order
       2. pizza_id – Unique code for each pizza type
       3. pizza_name_id – Standardized pizza name
       4. quantity – Number of pizzas ordered
       5. order_date – Date of the order
       6. order_time – Time of the order
       7. unit_price – Price per pizza
       8. total_price – Total price for the order line
       9. pizza_size – Size of the pizza (e.g., S, M, L)
       10. pizza_category – Category of the pizza (e.g., Classic, Veggie, Supreme)
       11. pizza_ingredients – List of ingredients used in each pizza

# 6. Tool used:- Power Bi

# 7. DAX used:-

   1. AVG ORDER QTY = [TOTAL ORDER QTY]/[Total orders]
   2. hour = HOUR(pizza_sales[only_time])
   3. revenue/month = CALCULATE(sum(pizza_sales[total_price])/DISTINCTCOUNT(pizza_sales[Month_name]))
   4. revenue/orders = [Total revenue]/[Total orders]
   5. TOTAL ORDER QTY = DISTINCTCOUNT(pizza_sales[pizza_id])
   6. Total revenue = ROUNDUP(sum(pizza_sales[total_price]),0)
   7. total_month = DISTINCTCOUNT(pizza_sales[Month_name])

# 8. KPIs:-

1. Total Orders
   What is the total number of pizza orders placed?
2. Total Revenue
   How much total revenue has the pizza shop generated?
3. Total Order Quantity
   How many pizzas were sold in total?
4. Revenue per Order
   What is the average revenue generated per order?
5. Time-Wise Sales
   At what time of the day are most pizzas sold?
6. Monthly Sales Trends
   How does sales performance vary month by month?
7. Day-Wise Sales Trends
   Which days of the week have the highest and lowest sales?
8. Pizza Orders by Category
   Which pizza category (e.g., Classic, Veggie, Supreme) is most popular?
9. Yearly Sales Amount by Pizza Size
   How much revenue is generated yearly across different pizza sizes?
10. Top-Selling Pizzas (by Revenue)
   Which pizzas generate the most revenue?
11. Top-Selling Pizzas (by Quantity)
   Which pizzas are sold the most in terms of quantity?
12. Least-Selling Pizzas (Overall)
   Which pizzas have the lowest sales performance?
13.Least-Selling Pizzas by Category
   Within each category, which pizzas perform the worst?
14. Most and Least Ordered Pizzas (by Order Count)
   Which pizzas are ordered the most and least in terms of order frequency?

# 9. Conclusion:-
The Pizza Shop Sales Analysis project successfully transformed raw sales data into meaningful business insights using Power BI. By analyzing key metrics such as total revenue, order quantity, sales trends, and pizza performance, the report provides a clear picture of customer preferences and sales dynamics.
Interactive dashboards and visualizations enabled a deep dive into time-based trends, category-wise sales, and top-performing products, helping identify both strengths and areas of improvement. These insights empower decision-makers to optimize inventory, enhance menu offerings, and implement targeted marketing strategies.
Overall, the project demonstrates how data-driven analysis can significantly improve operational efficiency and support strategic planning for a food and beverage business.
















           
