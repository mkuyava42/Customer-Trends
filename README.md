# Customer Shopping Behavior Analysis

An end-to-end analysis of 3,900 retail transactions, exploring what separates a loyal customer from a one-time buyer and where subscription, discount, and shipping strategy could better drive retention.

## Overview

**Business question:** Which factors — subscription status, discounting, shipping speed, purchase frequency — actually correlate with a customer moving from "new" to "returning" to "loyal," so marketing spend can follow the signal instead of a hunch?

**Approach:** Clean and explore the transaction data in Python, segment customers by loyalty tier, then build two dashboards — one internal/filterable (Power BI), one public/shareable (Tableau Public) — to surface the findings for different audiences.

## Dataset

- **Rows:** 3,900 transactions
- **Fields:** 20, including age, gender, item purchased, category, purchase amount, location, review rating, subscription status, shipping type, discount applied, previous purchases, payment method, purchase frequency, and customer segment
- **Categories:** Clothing, Accessories, Footwear, Outerwear

## Tools

| Purpose | Tool |
|---|---|
| Data cleaning & EDA | Python (pandas) |
| Internal dashboard | Power BI |
| Public dashboard | Tableau Public |
| Source data | CSV export |

## Process

1. **Clean & profile**  loaded the export in pandas, standardized column naming and category labels, checked for duplicates/nulls, and profiled distributions for purchase amount, rating, and frequency.
2. **Segment the customer base**  grouped customers into New, Returning, and Loyal segments and cross-tabbed each against subscription status, discount usage, and shipping type.
3. **Build the dashboard**  modeled the cleaned table in Power BI for a filterable internal view (by category, region, segment), then rebuilt the headline visuals in Tableau Public for a shareable, embeddable version.

## Key findings

- **Loyalty is the default outcome, not the exception**  62% of customers are already classified Loyal versus just 1% New, reframing the analysis toward retention rather than acquisition.
- **Subscriptions are underused**  only 26% of customers are subscribed, despite subscribers skewing toward the loyal segment, pointing to a clear upsell opportunity.
- **Purchase cadence clusters around quarterly**  the most common repurchase interval is quarterly or annual rather than monthly, suggesting lifecycle campaigns should be timed to a 3-month cycle.
- **Clothing dominates volume**  Clothing accounts for 44% of all transactions, more than double the next category (Accessories, 32%), giving category-level promotions outsized reach if targeted at Clothing first.

## Headline numbers

| Metric | Value |
|---|---|
| Transactions | 3,900 |
| Avg. purchase | $60.05 |
| Avg. review rating | 3.69 / 5 |
| Loyal segment | 62% |
| Subscribed | 26% |

## Repo contents

- `customer_export.csv` — cleaned source data
- `Customer_Trends_Dashboard.pbix` — Power BI dashboard
- `Customer_Trends.twb` — Tableau workbook
- `Customer_Shopping_Behavior_Analysis.pptx` — summary slide deck
- `customer_shopping_trends.ipynb` — Python EDA notebook

## Links

- Live Tableau dashboard: _add link once published to Tableau Public_

## Author

Marisa Kuyava 
