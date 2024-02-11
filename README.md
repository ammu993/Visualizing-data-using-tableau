# Visualizing data using Tableau

## Overview
Color-blind friendly Sales Overview Dashboard that not only showcases key performance indicators (KPIs) but also functions as a springboard for in-depth exploration. For instance, it serves as a starting point to delve into the investigation of factors contributing to the decline in average monthly sales since FY 2003, offering a comprehensive visualization for both explanatory and diagnostic analysis

## Project Structure
Connecting relevant data sources to create a dashboard for the fictitious AdventureWorks (Bikes and its accessories) company that offers an overview of the Sales between FY 2001-FY2004.

## Tools and Technologies
Tableau Public & BigQuery

## Data Source & Parameters 
AdventureWorks 2001-2004 dataset
* Period of analysis: FY 2002, FY 2003, FY 2004 (Fiscal years start on July 1st and end on June 30 the following year)
* Territory: US, CA, AU, GB, FR, DE
* Source: Internal Data of 'Adventure Works', 2001-2004
* Currency: USD or $
* Purpose: Internal use by sales department


## Data Cleaning and Preprocessing
To present data regarding top salespersons in each country and income earned through the sale of products ( categorized into Accessories, Bikes, Components, and Clothing), in BigQuery, I joined multiple tables to modify <kbd> adwentureworks_db.salesorderheader </kbd> and <kbd>adwentureworks_db.salesorderdetail</kbd> tables. The resulting tables were downloaded in .csv format and added as data sources to Tableau public.

## Analysis and Visualizations

For an interactive dashboard [click here](https://public.tableau.com/shared/T463DC9N8?:display_count=n&:origin=viz_share_link)  

![AdventureWorks Sales](https://github.com/ammu993/Visualizing-data-using-tableau/assets/74145869/0e728692-a98a-4737-ae77-16fefcf7d392)

[Sales across Geographical region with top salespersons of the country]![hover_topsalesperson](https://github.com/ammu993/Visualizing-data-using-tableau/assets/74145869/b5ace0f3-2bf5-40ed-b19f-9dc1116652d1)

## Insights
General insights gained from Dashboard that can be filtered on fiscal years of interest, sales type(online/offline), and country:  
* Total Revenue generated is $140.71M
* The count of online sales is much higher than offline sales. However, offline sales bring in higher revenue.
* Offline sales began only in FY2004 in Germany and Australia.
* USA is the highest revenue-generating market.
* In terms of which sales reason resulted in higher total revenue, "Price" occupies the first position.
* There is a drop in average online sales in July 2002 and July 2003.

[Drop in Average Online  Sales from July 2002 despite the increase in Total sales]  ![drop in average sales](https://github.com/ammu993/Visualizing-data-using-tableau/assets/74145869/492dd9d6-2505-4546-8ca6-230594bef425)  

Diagnostic analysis:  
**What caused the drop in average online sales at the beginning of FY 2003 though the total sales seemed to grow?**  
In FY 2002 and FY 2003, only  product categories ‘Bikes’ were sold online. From FY 2004, new product categories  ‘Accessories’ and ‘Clothing’ were being sold online. These are low-priced categories in comparison to ‘Bikes’. In the sales reason as % of Total Sales tables, new sales reasons such as TV ads, Price, Manufacturer, and Price also showed up in FY 2004. So, even though the sales increased, it was for goods that were priced low. Thus, drop in average sales. 

## Recommendations for Further Action
* A product category that is revenue-generating after Bikes and sold only offline is “Components”. Introducing sales of this category of goods in online sales, can help with increasing the overall average online sales in the upcoming FY 2005.  
* In AU and countries in Europe (DE, FR, GB)  improvement in online sales will be beneficial as most of their sales are done online. The online sales market seems to be gaining dominance in the US in FY 2004, so improving online sales would benefit this market as well.

## Challenges and Limitations
The KPIs shown and Filters include FY 2005 (though it contains only data from July 2004). This data can be omitted in further analysis as done in the "Yearly comparison of the Monthly Sales" chart.
