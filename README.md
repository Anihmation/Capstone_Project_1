# SUPERSTORE DATA ANALYSIS
![Superstore front picture](https://user-images.githubusercontent.com/78387629/185406525-a28f2914-2391-4fc9-a05f-99bf221d9e6b.png)

__A data analysis of a Superstore.__
___
## PROJECT DESCRIPTION
The Project Dataset collected is made up of 5 Workbooks titled: ‘Customers’, ‘Locations’, ‘Products’, ‘Sales Reps’ and finally ‘Sales’. The Customers workbook gives more detail to who a customer with 793entries under 3 columns; the Locations workbook gives more detail to the sales with 632 entries under 5 columns; the Products Workbook gives more detail to the Products with 1,894 entries under 4 columns; the Sales Reps Workbook gives detail to the Sales Reps with 14 entries under 4 columns and finally the Sales Workbook sums up the Sales with 9,994 entries under 12 columns.

Simply put, the Dataset is a Sales Report of this Superstore, that has operated in the whole of United States of America for 4 years.
I extracted, wrangled, and transformed the data to get it ready for the analysis. I used the Business Intelligence tool, Power BI to perform the ETL (Extract, Transform and Load), Data Query and EDA (Exploratory Data Analysis) and Data Visualization.
___
## DATA SOURCE
I sourced the data used from github. Here's the link:
- https://github.com/Fabulousnani/Data-Developer-Bootcamp/blob/main/SuperStore_Normalized.xlsx
___
## PROBLEM STATEMENT
The Business problem is the basically maximizing the Store’s Profit; and through my analysis, I would discover the determining factors of the revenue and derive a workable solution to scale it.
___
## DESIGN METHODOLOGY
I downloaded the raw file dataset to my PC from Github, hence creating a folder to serve as my local Datalake.
I then created a Power BI file to connect the dataset. I used Power BI to Explore, Transform and Load (ETL) the data. Herein I used the Power Query to clean the data as ought, which resulted in loading a 5 different Tables. I also used the tool to carryout my Exploratory Data Analysis (EDA) and Data Visualization.
After connecting the Excel Workbook to the Power BI in the Model Page, I observed the other 4 workbooks gives details to the Sales workbook but only 2 was in connection, seeing that Power Query gave ‘Products’ and ‘Customers’ Tables new headers. I quickly transformed the data using ‘Use First Row as Headers’ button in Power Query once more, afterwards every workbook connected to the ‘Sales’ Table.

I opened the Report Page where I carried out some DAX (Data Analysis Expressions) to ascertain variables that will help my analysis namely: the ‘Sales after Discount’, ‘Total Discount’, ‘Total Cost’, ‘Total Profit’, ‘Total Quantity’ and ‘Total Sales’. Afterwards I built the Data Visualizations in the Report Page. I did some formatting to the visuals, choosing the most suitable visual to present the Data. I also introduced slicers to enhance my visuals only in the first sheet. I also introduced Page navigation buttons in a ribbon to depict a Web App interface.
I also used basic PowerPoint knowledge to provide a few design elements to enhance the Data Visualization.
All this were used to dig deep into the data and arrive at insightful results

__DAX REFERENCE:__
- Welcome Text = VAR Hour = HOUR(Now()) VAR Greeting = SWITCH( TRUE(),
Hour >= 0 && Hour < 5, "Good Night,",Hour >= 5 && Hour < 12, "Good Morning,", Hour >= 12 && Hour < 16, "Good Afternoon,",Hour >= 16 && Hour < 24, "Good Evening,") RETURN Greeting & " " & SELECTEDVALUE ('Sales Reps'[Sales Rep])
- Total Cost = [Total Sales after Discount] - [Total Profit]
- Total Discount = SUM(Sales[Discount])
- Total Profit = SUM(Sales[Profit])
- Total Quantity = SUM(Sales[Quantity])
- Total Sales = SUM(Sales[Sales])
-Total Sales after Discount = [Total Sales] - [Total Discount]

___
## FINDINGS AND DATA ANALYSIS
![Superstore Analysis Welcome Page](https://user-images.githubusercontent.com/78387629/186147511-0d9d44e0-79fe-41d7-b73a-54e7dd09290f.jpg)

![Superstore Analysis Second Page](https://user-images.githubusercontent.com/78387629/186147544-8dd361f6-bbb0-4653-be2d-7ce525809182.jpg)

![Superstore Analysis Third Page](https://user-images.githubusercontent.com/78387629/186147586-e940e314-4e8e-4ef3-a78d-c63d7d076baf.jpg)

![Superstore Analysis Fourth Page](https://user-images.githubusercontent.com/78387629/186147632-53c52c90-6d54-4e48-8a5f-1ed3bd6d0a38.jpg)

-	The Business has been quite profitable over the four years, with a 10-20% increase per succeeding year.
-	The Superstores booms in California and New York the most, with a 74K and 76K profit respectively, making the two the most revenue generating States.
-	The Superstores suffers a great loss in Texas and Ohio the most, with a 26K and 17K loss respectively, making the two the least revenue generating States.
-	The total cost and total Profit over the months have a similar trendline, showing their relationship over the time being to be progressive in nature.
-	The Business makes the most Sales and Profit in the West Region with a 725K Sales over a 108k profit, whereas the business makes the least sales in the South Region of 391K but the least Profit in the Central Region of 39K.
-	Organic as a Sales Rep yields the most Profit of 183K, while Jessica Smith yields the least Profit of 2.95K.
-	The Standard Class, Ship Mode yields the most gain of 164K while The Same Day Ship Mode yields just about 16K.
-	The Consumer segment when it comes to Customers yields the most profit of 134k for the Business.
-	When it comes to Product Category, Technology yields the most Profit of 145K, while Furniture yields the least Profit of 18K.
-	When it comes to Sales Team Organic is matchless to Profit generation.
___
## RECOMMENDATION
___
## CONCLUSION
In conclusion, I will say if all these recommendations of mine are implemented appropriately, the business revenue will be maximized greatly from a 10% annual increase to about 40% annual increase. As one can vividly see how the data analysis has been essential in determining the Factors to maximizing the business revenue.___
### ATTRIBUTION
- The Introductory picture was gotten from Tima Miroshnichenko at Pexels.
- The icons used is attributed to Unicode
- The dataset I used for the work is attributed to https://github.com/Fabulousnani
___
