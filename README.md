# Visualizing data using Tableau

## Overview
Color-blind friendly Sales Overview Dashboard that not only showcases key performance indicators (KPIs) but also functions as a springboard for in-depth exploration. For instance, it serves as a starting point to delve into the investigation of factors contributing to the decline in average monthly sales since FY 2, offering a comprehensive visualization for both explanatory and diagnostic analysis

## Project Structure
Connecting relevant data sources to create a dashboard for the fictitious AdventureWorks (Bikes and its accessories) company.

## Tools and Technologies
Tableau Public & BigQuery

## Data Source & Parameters 
AdventureWorks 2001-2004 dataset
* Period of analysis: FY 2002, FY 2003, FY 2004 (Fiscal years start on July 1st and end on June 30 the following year)
* Territory: US, CA, AU, GB, FR, DE
* Source: Internal Data of 'Adventure Works', 2001-2004
* Currency: USD or $
* Purpose: Internal use by sales department
* KPIs: Total revenue, Average Order Value, Number of Orders, Average days to ship

## Data Cleaning and Preprocessing
In BigQuery, the additional data sets were extracted to show product sales by category.

## Analysis and Insights
The following question was posed which led to diagnostic analysis and insight:

**What caused the drop in average online sales at the beginning of FY 2004 though the total sales seemed to grow?**

In FY 2002 and FY 2003, only  product categories ‘Bikes’ were sold online. From FY 2004, new product categories  ‘Accessories’ and ‘Clothing’ were being sold online. These are low-priced categories in comparison to ‘Bikes’. In the sales reason as % of Total Sales tables, new sales reasons such as TV ads, Price, Manufacturer, and Price also showed up in FY 2004. So, even though the sales increased, it was for goods that were priced low. Thus, drop in average sales. 

## Visualizations
For interactive dashboard [click here](https://public.tableau.com/shared/T463DC9N8?:display_count=n&:origin=viz_share_link)
<br>
![AdventureWorks Sales](https://github.com/ammu993/Visualizing-data-using-tableau/assets/74145869/0e728692-a98a-4737-ae77-16fefcf7d392)

## Challenges and Limitations
The KPIs shown and Filters include FY 2005 (contains only data from July 2004). This data can be omitted in further analysis as done in the "Yearly comparison of the Monthly Sales" chart.
