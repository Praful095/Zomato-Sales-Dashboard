# Zomato-Sales-Dashboard

#  Zomato Sales Tracking and Analysis Dashboard

## Problem Statement

Zomato, a leading food delivery and restaurant discovery platform, operates in numerous cities and offers a wide variety of cuisines. With a vast number of orders placed daily, it becomes essential for Zomato to efficiently track and analyze sales data, customer ratings, and other key performance metrics. This analysis is crucial to identify trends, optimize menu offerings, and enhance customer satisfaction.

The objective is to create a Power BI dashboard that provides Zomato with detailed insights into their sales performance, customer ratings of menu items, revenue generated, quantity sold, and top-performing cities. The dashboard should enable Zomato to monitor these metrics in real-time, identify areas for improvement, and make data-driven decisions to enhance their operations and customer experience.






### Steps followed Creating a Power BI Dashboard for Zomato Sales Dashboard
To create a Power BI dashboard that tracks and analyzes Zomato  sales using the provided order and details CSV files, follow these steps:

1. Load Data into Power BI
Open Power BI Desktop.
Import CSV Files:
Go to Home > Get Data > Text/CSV.
Select the order.csv file and click Open.
Repeat the process for the details.csv file.
2. Data Preparation and Cleaning
Examine the Data:

Click on Data view to inspect the loaded data for both order and details tables.
Renamed Columns as required

Ensured that column names are clean and consistent.
 
Created Relationships:

1) created relationship between the orders (r_id) and restaurant(r_id)
2) the second relationship is establ;ished between oreders(r_id) & menu(r_id)

Go to Model view.
Drag and drop order_id from the order table to the details table to create a relationship.
Transform Data (if needed):

Go to Home > Transform Data to open Power Query Editor.
Apply any necessary transformations such as removing duplicates, handling missing values, or changing data types.
3. Create Calculated Columns and Measures
Calculated Columns:

Create calculated columns for additional insights if needed, such as Year or Month from order_date.
Measures:

Create measures for key metrics like total sales, ratings count, orders count,topN-Sales etc.

DAX
Copy code:

Total Sales = SUM( orders[Value])

orders count = Orders_count = COUNT(orders[Value]) 

ratings count = Rating_count = COUNT(restaurant[rating])


4. Build the Dashboard
Sales Performance Overview:

created visuals like Line Charts, Bar Charts, and Cards to display total sales, profit, and quantity over time.
Use the order_date field to show trends over different periods.
Geographical Analysis:

![](https://github.com/Praful095/Zomato-Sales-Dashboard/assets/158684580/ab9b2c1c-9a4a-4c8b-ab3d-4edd1a5e4038)

Useed bar graph in order to determine the sales by city

![](https://github.com/Praful095/Zomato-Sales-Dashboard/assets/158684580/803c0447-03e2-4be5-98f5-310fa23e2edf)



category analysis and ratings:
used calculations for analysing the catoegories of and their ratiing by virtue of amount and quantity sold

![](https://github.com/Praful095/Zomato-Sales-Dashboard/assets/158684580/a90f3a7b-1769-46c9-ad85-8296234e2452)



Use Line Charts and Area Charts to display sales trends over different periods.
Highlight peak sales periods and compare them to off-peak periods.

![](https://github.com/Praful095/Zomato-Sales-Dashboard/assets/158684580/b15faa94-9824-499f-8958-57725ff42596)

5. Enhance and Customize the Dashboard:

Add slicers for order_date, state, city, category, and sub_category to enable dynamic filtering.

![](https://github.com/Praful095/Zomato-Sales-Dashboard/assets/158684580/f78bd9f8-eedd-4763-8205-93d1f4ff4fa9)
![](https://github.com/Praful095/Zomato-Sales-Dashboard/assets/158684580/b454032f-768c-4183-9500-a6a040a6d9be)

Design and Format:


Customize the dashboard layout, color scheme, and fonts to make it visually appealing.
Use consistent formatting for easier interpretation of data.
Added Titles and Labels:

Ensured all visuals have clear titles and labels.
Added tooltips to provide additional context for the data points.
 

# Snapshot of Dashboard (Power BI Service)

![Dashboard Snapshot](https://github.com/Praful095/Zomato-Sales-Dashboard/assets/158684580/3f4dbda0-cd02-4c9f-83c3-3264d720f9da)



# Insights
# the Overview:

# Total Amount Generated :
 The dashboard shows that Zomato has generated a total sales amount of 989M.

 #  Total Quantity sold :
 The total quantity of items sold is 2M.

# Total Ratings:
 Zomato has received a total of 148K ratings.

 # Total orders:
The total number of orders placed is 150K.
# Geographical Analysis:

Top Cities by Amount:

The bar chart on the right highlights the top cities based on the amount generated. The top cities include:
Tirupati
Electronic City
Baner, Pune
Rajpur
Others (various smaller cities or unspecified regions)
Tirupati is the leading city in terms of the amount generated.

# Sales Breakdown by Food Category:
Category-Wise Sales and Ratings:

Vegetarian Food:

Amount: 106M

Ratings: 10K

Non-Vegetarian Food:

Amount: 122M

Ratings: 12K

Other Food Categories:

Amount: 24M

Ratings: 927

# Sales Trends Over Time:
Sales by Year:

The line chart at the bottom right shows the sales trend from 2017 to 2020:

2017: Sales amount was approximately 0.09B.

2018: Sales increased significantly to 0.41B.

2019: Sales slightly decreased to 0.34B.

2020: Sales dropped to 0.14B.

The peak year for sales was 2018, after which there was a decline.


# Insights Summary

High Revenue Cities: Tirupati leads in terms of the amount generated, followed by Electronic City and Baner, Pune.

Popular Food Categories: Non-vegetarian food generates the highest amount (122M) and receives the most ratings (12K), followed by vegetarian food.

Sales Performance: There was a significant growth in sales from 2017 to 2018, peaking in 2018. However, there has been a decline in sales in the subsequent years, particularly in 2020.

Customer Engagement: The number of ratings suggests active
 customer engagement, with 148K ratings given across all orders.

# Zomato Sales-Dashboard.md.txt
Displaying # Zomato Sales-Dashboard.md.txt.



