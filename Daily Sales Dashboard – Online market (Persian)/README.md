BI Dashboards and KPIs
1. BI Dashboards (Power BI)
General Dashboard for Detailed Metrics

The goal of this dashboard is to provide business leaders with deep visibility into all aspects of the business and to uncover hidden trends.

Key Features:

Sales Overview → total sales, total orders, unique customers, average basket value.

Customer Behavior → new vs. returning customers, repeat purchases, daily/weekly active users.

Discount Analysis → sales split by product discount, coupon, voucher, and no discount.

Operational Metrics → % of delayed orders, % of changed orders, free delivery usage.

Top Performance → top 10 vendors, top 10 products, and revenue distribution by category/sub-category.

Visual Elements:

KPI Cards for high-level metrics.

Line Charts for sales trends over time.

Pie/Donut Charts for discount type breakdown and customer segments.

Bar Charts for top vendors, top products, and supermarket type comparison.

Map Visualizations for city/area-level sales.

Competitive Analysis Dashboard (Type 1 vs. Type 2 Supermarkets)

The second dashboard provides competitive insights between Type 1 and Type 2 supermarkets.

Key Insights:

Compare sales volumes and average order value (AOV) between the two types.

Evaluate promotion strategies (coupon, voucher, free delivery) and their impact on revenue.

Identify growth opportunities for Type 1 by simulating successful Type 2 strategies.

Highlight the potential uplift in sales if Type 1 adopts similar campaigns.

Visual Elements:

Clustered Bar/Column Charts → sales & AOV comparison.

Stacked Area Chart → discount contribution over time.

Scenario Simulation Table → projected financial impact of coupon/free delivery adoption.

Trend Lines → show before/after effects of promotions.

Data Modeling (Star Schema)

A dimensional star schema is designed to support BI reporting:

FactOrders → sales, quantity, discounts, flags.

DimDate → date, week, month, quarter, year, is_weekend.

DimCustomer → customer_id, segment, city_id, signup_date, lifetime_value.

DimProduct → product_id, category, sub-category, vendor_id.

DimVendor → vendor_id, vendor_name, vendor_region.

DimLocation → city_id, area_id, city_name, area_name.

DimCampaign → campaign_id, type (coupon/free delivery), start_date, end_date.

This structure ensures:

Fast aggregation for recurring reporting.

Flexibility in slicing and dicing data.

Easy integration with forecasting outputs.

2. Key Performance Indicators (KPIs)

Below are 30 essential KPIs designed for this dataset and business case.

Sales KPIs

Total Sales Revenue → overall sales value, main measure of financial success.

Company Market Share (Revenue %) → company sales vs. total market sales.

Number of Active Vendors → total unique vendors; measures supplier network size.

Sales from Promotions & Free Delivery → revenue driven by marketing campaigns.

Product KPIs

Total Units Sold → volume of products sold (ignores price).

Unique Products Sold → product diversity in sales.

Number of Product Categories Sold → variety of product categories contributing to sales.

Number of Sub-Categories Sold → deeper product assortment.

Customer KPIs

Total Unique Customers → total number of buyers.

Average Purchases per Customer → customer loyalty metric.

Returning Customers (2+ purchases) → recurring buyers indicating sustainable revenue.

Number of Cities with Active Sales → geographic market coverage.

Order KPIs

Total Orders → total recorded transactions.

Average Order Value (AOV) → average sales value per order.

Average Sales of Top 10 Vendors → concentration of sales among leading vendors.

Average Vendor Sales → fairness of distribution across all vendors.

Marketing KPIs

Sales from Campaigns & Free Delivery → revenue impact of promotional activities.

Sales from Discounted Products → sales uplift from promotions.

Total Discount Amount → total cost of discounts given.

Unique Discounted Products → number of different products sold with a discount.

Operational KPIs

Number of Delayed Orders → logistics/fulfillment problems.

Number of Changed Orders → orders altered during fulfillment.

Value of Delayed Orders → sales value tied to delayed deliveries.

Value of Changed Orders → financial impact of changed orders.

Analytical & Comparative KPIs

Sales by Vendor → vendor contribution to revenue.

Sales by Product Category → demand distribution by product group.

Sales by Geography (City/Area) → market reach by region.

Sales by Customer Type (New vs Returning) → revenue split by customer loyalty.

Sales by Supermarket Type (1 vs 2) → competitive positioning.

Sales by Discount Type → breakdown by product discount, coupon, voucher, or no discount.

Together, these dashboards and KPIs provide a full analytical framework:

Business leaders can monitor financial performance, customer loyalty, and operations.

Competitive analysis enables Type 1 supermarkets to simulate and adopt strategies from Type 2.

Star schema modeling and forecasting integration ensure the system is scalable, repeatable, and BI-ready.
