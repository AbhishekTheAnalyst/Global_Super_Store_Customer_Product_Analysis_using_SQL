# Global-Super-Store-Customer-Product-Analysis

**Analysis**
--------------------------------------------------------------------------------------------------------------------------

1.)	**Retrieving all Columns from Global Superstore Data**

**SELECT** *

**FROM** [Global Superstore data]

![image](https://github.com/AbhishekTheAnalyst/Global_Super_Store_Customer_Product_Analysis_using_SQL/assets/109465334/e1cab174-16f4-4585-9287-8ce9106ae503)


2.)	**Top 5 Customers by Total Sales**

--Selecting the Customer Name and calculating the total sales by using the sum function from the 'Global Superstore' table.

--Selecting the Top 5 Customers.

**SELECT TOP 5** Customer_Name, **ROUND(SUM**(Sales), 2) **AS** Total_Sales

--Retrieving the data from the ‘Global Superstore’ Table.

**FROM** [Global Superstore data]

--Grouping the results by the Customer name.

**GROUP BY** Customer_Name

--Ordering the results by Total Sales in Descending order.

**ORDER BY** Total_Sales **DESC**;

![image](https://github.com/AbhishekTheAnalyst/Global_Super_Store_Customer_Product_Analysis_using_SQL/assets/109465334/8cae48bb-7c9c-4ae5-886d-a75cf64455f0)

3.)	**Top 5 Customers by Total Profit**

--Selecting the Customer Name and calculating the total profit by using the sum function from the 'Global Superstore' table.

--Selecting the Top 5 Customers.

**SELECT TOP 5** Customer_Name, **ROUND(SUM**(Profit),2) **AS** Total_Profit

--Retrieving the data from the ‘Global Superstore’ Table.

**FROM** [Global Superstore data]

--Grouping the results by the Customer name.

**GROUP BY** Customer_Name

--Ordering the results by Total Profit in Descending order.

**ORDER BY** Total_Profit **DESC**;

![image](https://github.com/AbhishekTheAnalyst/Global_Super_Store_Customer_Product_Analysis_using_SQL/assets/109465334/cfe533ba-8ce2-44f5-b7a6-7d116330c78b)

4.)	**Total Sales and Profit by Segment.**

--Selecting the Segment and calculating the total sales & profit by using the sum function from the 'Global Superstore' table.

**SELECT** Segment, **ROUND(SUM**(Sales), 2) **AS** Total_Sales, **ROUND(SUM**(Profit), 2) **AS** Total_Profit

--Retrieving the data from the ‘Global Superstore’ Table.

**FROM** [Global Superstore data]

--Grouping the results by Segment.

**GROUP BY** Segment

--Ordering the results by the Total_Profit.

![image](https://github.com/AbhishekTheAnalyst/Global_Super_Store_Customer_Product_Analysis_using_SQL/assets/109465334/af47ea5a-0ad6-4490-b150-cf01a5eb4fdd)

5.)	**What is the distribution of customers and total orders placed across different segments (e.g., consumer, corporate, home office)?**

--Selecting the Segment and calculating the count of distinct customer ID and count of orders from the 'Global Superstore' table.

**SELECT** Segment, **COUNT (DISTINCT** Customer_ID) **AS** Customer_Count, **COUNT**(Order_ID) **AS** Total_Orders_Placed

--Retrieving the data from the ‘Global Superstore’ Table.

**FROM** [Global Superstore data]

--Grouping the results by Segment.

**GROUP BY** Segment

--Ordering the results by the Count of Distinct Customers in Descending order.

**ORDER BY** Customer_Count **DESC**, Total_Orders_Placed;

![image](https://github.com/AbhishekTheAnalyst/Global_Super_Store_Customer_Product_Analysis_using_SQL/assets/109465334/f6edf3f5-25fa-47c7-8e20-4011de20ecc6)

6.)	**Which are the top 10 countries with the highest number of customers?**

--Selecting the TOP 10 Countries and calculating the count of distinct customer ID as Total Customers from the 'Global Superstore' table.

**SELECT TOP 10** Country, **COUNT(DISTINCT** Customer_ID) AS Total_Customers

--Retrieving the data from the ‘Global Superstore’ Table.

**FROM** [Global Superstore data]

--Grouping the results by Country.

**GROUP BY** Country

--Ordering the results by the Count of Distinct Customers in Descending order.

**ORDER BY** Total_Customers **DESC**;

![image](https://github.com/AbhishekTheAnalyst/Global_Super_Store_Customer_Product_Analysis_using_SQL/assets/109465334/56335095-502c-4b5c-b22b-9188527a3ef3)

7.) j

