# Global-Super-Store-Customer-Product-Analysis

**Analysis**
--------------------------------------------------------------------------------------------------------------------------

1.)	**Retrieving all Columns from Global Superstore Data**

SELECT *

FROM [Global Superstore data]

![image](https://github.com/AbhishekTheAnalyst/Global_Super_Store_Customer_Product_Analysis_using_SQL/assets/109465334/e1cab174-16f4-4585-9287-8ce9106ae503)


2.)	**Top 5 Customers by Total Sales**

--Selecting the Customer Name and calculating the total sales by using the sum function from the 'Global Superstore' table.

--Selecting the Top 5 Customers.

SELECT TOP 5 Customer_Name, ROUND(SUM(Sales), 2) AS Total_Sales

--Retrieving the data from the ‘Global Superstore’ Table.

FROM [Global Superstore data]

--Grouping the results by the Customer name.

GROUP BY Customer_Name

--Ordering the results by Total Sales in Descending order.

ORDER BY Total_Sales DESC;

![image](https://github.com/AbhishekTheAnalyst/Global_Super_Store_Customer_Product_Analysis_using_SQL/assets/109465334/8cae48bb-7c9c-4ae5-886d-a75cf64455f0)

3.)	**Top 5 Customers by Total Profit**

--Selecting the Customer Name and calculating the total profit by using the sum function from the 'Global Superstore' table.

--Selecting the Top 5 Customers.

SELECT TOP 5 Customer_Name, ROUND(SUM(Profit),2) AS Total_Profit

--Retrieving the data from the ‘Global Superstore’ Table.

FROM [Global Superstore data]

--Grouping the results by the Customer name.

GROUP BY Customer_Name

--Ordering the results by Total Profit in Descending order.

ORDER BY Total_Profit DESC;

![image](https://github.com/AbhishekTheAnalyst/Global_Super_Store_Customer_Product_Analysis_using_SQL/assets/109465334/cfe533ba-8ce2-44f5-b7a6-7d116330c78b)

4.)	**Total Sales and Profit by Segment.**

--Selecting the Segment and calculating the total sales & profit by using the sum function from the 'Global Superstore' table.

SELECT Segment, ROUND(SUM(Sales), 2) AS Total_Sales, ROUND(SUM(Profit), 2) AS Total_Profit

--Retrieving the data from the ‘Global Superstore’ Table.

FROM [Global Superstore data]

--Grouping the results by Segment.

GROUP BY Segment

--Ordering the results by the Total_Profit.

ORDER BY Total_Profit DESC;

![image](https://github.com/AbhishekTheAnalyst/Global_Super_Store_Customer_Product_Analysis_using_SQL/assets/109465334/f6edf3f5-25fa-47c7-8e20-4011de20ecc6)



