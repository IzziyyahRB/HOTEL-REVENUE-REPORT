# HOTEL-REVENUE-REPORT
This is a mini-SQL project showing basic Data cleaning and Exploratory Data Analysis with SQL and visualizations from this data with Power Bi. This repo consists of an Excel file, SQL query file and Power Bi report file in pdf format.

Presented with a hotel’s data in an excel spreadsheet, I was to carry out the following tasks:
-	Build a database with the excel dataset in an SQL server.
-	Develop the SQL Query for EDA
-	Connect Database to Power Bi
-	Visualize data in Power Bi
-	Summarize findings


**PROBLEM STATEMENT**

Stakeholders want to know the following:

1.	Is our hotel revenue growing?
2.	Should we increase our parking lot size?
3.	What trends can we see in our data?


**Build a database with the excel dataset in an SQL server**

After downloading the excel file, I looked through it to have an idea of what the dataset looks like and what it comprises of i.e the columns and what it means.

I also scanned for missing/null values. Dataset has 5 sheets in the excel workbook which are 2018, 2019, 2020, meal_cost and market_segment. 2018, 2019 and 2020 sheets comprises of the same 32 columns while meal_cost and market_segment comprise of 2 columns each.

To build this as a database using SQL Server Management Studio, I connected my excel file to the SQL server by the following steps:

-	Right-click on databases > New Database > Add Database Name and Click OK > Right-click on the New Databse created > Select Tasks > Import Data > Select Next > Select Microsoft Excel as Data Source > Select Excel version > Click Next and Select Destination > Click Next then Finish. The data has now been imported to the created database.


**Develop the SQL Query for EDA**

Check the hotel revenue query file in the repository.

**Connect Database to Power Bi**

- From the Power Bi Home Tab > Click on Get Data > Select SQL Server > Fill in Server Name(this pops up when you open the SQL Server Management Studio) and Database > Select Import > Click on Advanced options > Copy and Paste SQL Query in the SQL statement box > Include relationship columns > Click OK
Automatically data from Database uploads to Power Query and then loaded to Power Bi to create visualizations with it.


**Visualize data in Power Bi**

I created visualizations like Line Charts, Slicers, Tables, Matrix and Cards to answers the following questions:
1.	Is our hotel revenue growing?
2.	Should we increase our parking lot size?
3.	What trends can we see in our data?


**Summarize findings**

1.	From the Line Chart and the Matrix, the hotel is experiencing an increase in revenue per year (although the 2020 data doesn’t contain all the months of the year), it’s still higher than the previous years.
2.	From the data about 2% of all stay-ins use the parking lot which isn’t much of a significant amount and this percentage has remained consistent through the years. This was illustrated in the Matrix visual. I would say the parking lot size should be left as it is or even down-sized.
3.	There is an p-trend in the number of nights spent in the hotel which explains increase in revenue. The average of discounts has remained constant over the years and the cost of average daily rate maintains a constant pattern. 
