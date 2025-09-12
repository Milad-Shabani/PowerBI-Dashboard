BI Dashboards (Power BI)
1. General Dashboard for Detailed Metrics

The purpose of this dashboard is to give business leaders deep visibility into key metrics and allow them to identify hidden trends.
Key features:

Sales Overview → total sales, total orders, unique customers, average basket value.

Customer Behavior → new vs. returning customers, repeat purchases, daily/weekly active users

Discount Analysis → sales split by product discount, coupon, voucher, and no discount.

Operational Metrics → % of delayed orders, % of changed orders, free delivery usage.

Top Performance → top 10 vendors, top 10 products, and revenue distribution by category/sub-category.

Visual elements:

KPI Cards for high-level metrics.

Line Charts for sales trends over time.

Pie/Donut Charts for discount type breakdown and customer segments.

Bar Charts for top vendors, top products, and sales by supermarket type.

Map Visualization for city/area-level sales.

2. Competitive Analysis Dashboard (Type 1 vs Type 2 Supermarkets)

The second dashboard focuses on competitive insights between Supermarket Type 1 and Type 2.

Key insights:

Compare sales volumes and average order value (AOV) between the two types.

Analyze promotion strategies (coupon, voucher, free delivery) and their impact on revenue.

Identify growth opportunities for Type 1 by simulating Type 2 strategies (e.g., adopting coupons, targeted free delivery).

Highlight the potential uplift in sales if Type 1 implements similar campaigns.

Visual elements:

Clustered Bar/Column Charts → sales & AOV comparison between Type 1 and Type 2.

Stacked Area Chart → discount type contribution to sales over time.

Scenario Simulation Table → financial impact of coupon/free delivery adoption for Type 1.

Trend Lines → show before/after effect of promotions.

3. Data Modeling for BI

To support dashboards, a dimensional star schema is designed:

FactOrders (measures: sales, quantity, discounts, flags).

Dimensions: Date, Customer, Product, Vendor, Location, Campaign.

This structure ensures:

Fast aggregation for recurring reporting.

Flexibility in slicing/dicing (by customer, product, city, promotion).

Easy integration with forecasting outputs.

4. Outputs for BI Consumption

Power BI dashboards are connected to the processed dataset (with derived columns like Discount Type).

Forecasting results (from Python/R pipeline) are stored in FactForecast and visualized alongside actuals.


All KPIs and dashboards are designed to be interactive and support drill-down analysis.
