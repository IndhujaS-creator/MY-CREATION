/*#Superstore
https://github.com/IndhujaS-creator
*/

CREATE TABLE superstore(
	Row_ID SERIAL,
	Order_ID VARCHAR(35),
	Order_Date DATE,
	Ship_Date DATE,
	Ship_Mode VARCHAR(35),
	Customer_ID VARCHAR(35),
	Customer_Name VARCHAR(50),
	Segment VARCHAR(35),
	Country VARCHAR(40),
	City VARCHAR(40),
	State VARCHAR(40),
	Postal_Code NUMERIC,
	Region VARCHAR(15),
	Product_ID VARCHAR(40),
	Category VARCHAR(50),
	Sub_Category VARCHAR(50),
	Product_Name VARCHAR(200),
	Sales NUMERIC,
	Quantity NUMERIC,
	Discount NUMERIC,
	Profit NUMERIC
	)
--Adding csv
COPY superstore 
FROM E:\Alma2\Interview question
WITH (FORMAT CSV, HEADER);

--Checking superstore
SELECT *
FROM superstore;
