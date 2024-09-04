# Data_Warehousing_Concepts

**Data Warehouse :** A data warehouse is a centralized repository that stores large volumes of data from various sources within an organization. 
**Database:** A database is an organized collection of data that is stored and managed to allow easy access, retrieval, and manipulation.
**Datamart:** A data mart is a subset of a data warehouse that is focused on a specific business area, department, or function within an organization. 
**Datalake:** A data lake is a centralized repository that allows you to store vast amounts of raw data in its native format, including structured, semi-structured, and unstructured data.

**Types of tables:**
1. Dimension table: Gives context to fact tables like ProductID, CustomerID...
2. Fact table: It stores quantitaive measures. Like SalesAmount, QuantitySold..

**Types of facts:**
1. Additive: Performs all aggregation functions eg., min,max,count,avg, - quantities sold in a month
2. Semi-Additive: Performs few aggregation functions eg., min & max - bank balance
3. Non-Additive: Cannot perform any aggregation functions eg., ratio, percentages

**Types of Dimensions:**
1. Slowly Changing : Changes slowly i.e., address
2. Conformed : Used by mutliple facts i.e., time shared among multiple tables
3. Degenerate : Fact table stores dimension values i.e., invoice number
4. Junk : Combines two or more related low cardinality flags into a single dimension. i.e., T/F , 1/0 
5. Role-playing : Date plays different roles in different tables. i.e., Ordered date, Shipped date...
6. Static : Does not change eg., Gender
7. Shrunken : Dimension further divided into smaller dimenions.

**Types of fact tables:**
1. Transaction Fact: Contains individual transaction info.
2. Periodic Snapshot: Contains summarized data within specific interval of time
3. Accumulating Snapshot: Designed to track changes i.e., ordered date, shipped, delivered
4. Factless fact: Don't have any facts i.e., just has all dim values like prodid, custid...


