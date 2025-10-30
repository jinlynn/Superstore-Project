# 🛒 Customer Segmentation & Sales Analysis: Superstore Dataset

## 📌 Project Overview
A customer segmentation and sales analysis project using the Superstore dataset from Kaggle ([link](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final/data)). The dataset contains with 9,994 transactions from 2014 to 2017. It includes information on sales, profit, orders, products, states, and customer details.

The project combines unsupervised clustering and an interactive dashboard to derive actionable insights for business strategy.

🔗 **Interactive Dashboard**: [View on Tableau Public](https://public.tableau.com/views/SuperstoreDashboard_17588127803760/Home?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## 🎯 Objectives
- Segment customers based on recency, frequency and monetary value (referred to as ‘customer cluster’)
- Recommend tailored strategies for each customer cluster.
- Analyse trends in sales and profitability across products and their categories, states, and customer segments and clusters.
- Find opportunities for growth and areas that require attention.

## 📁 Files and Structure
- images — Visuals used in the README
- `superstore_clustering.ipynb` — Notebook for clustering
- `README.md` — Project overview and documentation

## 🏡 Page 1: Home — Overall Business Overview

_Snapshot of Dashboard - Home:_

<img src="/images/Home.png" alt="Snapshot of Dashboard - Home" width="80%"/>

**Main KPIs:**

- Total revenue, profit, number of orders, average order value, with respective YoY changes

**Key Visuals & Features:**

- Trendlines for sales, profit, order volume, and average order value
- Product category revenue/profit view (clickable for filtering)
- Top 5 states by revenue (bar plot and interactive map)
- Order volume, revenue contribution, and average shipping days for each shipping mode

**Key Insights:**

- Revenue, profit, and no. of orders have been increasing YoY, but average order value is declining — number of orders have been increasing at a higher rate than order value.

**Recommended Actions:**

- Investigate factors contributing to declining order value (eg. discounting or smaller basket sizes)

## 🧑‍🧑‍🧒‍🧒 Page 2: Regional / Customer — Customer Analysis

_Snapshot of Dashboard - Regional/ Customer:_

<img src="/images/Regional_Customer.png" alt="Snapshot of Dashboard - Regional/ Customer" width="80%"/>

**Key Visuals & Features:**

- Revenue and profit by customer segment (click on segment to filter)
- Revenue by states
- Revenue from each customer cluster (in selected year only)
- RFM (Recency, Frequency, Monetary) breakdown for customer clusters (historical)
- Top 5 states by revenue, profit, and order volume

**Key Insights:**

- Consumers contribute the most to revenue and profit
- Customer clusters identified: Nurture, Reward, Re-engage, Reconnect
- ‘Reward’ customers: 43% of base → 66% of revenue
- ‘Nurture’ customers: 45% of base → 29% of revenue

**Recommended Actions:**

| **Customer Segment** | **Insight Summary** | **Goal** | **Recommended Actions** |
|:----------------------|:--------------------|:----------|:-------------------------|
| **Nurture** | New, low-value, infrequent buyers with limited interaction | Convert first-time buyers into repeat customers | Offer limited-time discounts on next purchase.<br>Use targeted “frequently bought together” recommendations.<br>Launch a referral rewards program to build familiarity and trust. |
| **Reward** | High-value, loyal customers with strong engagement and frequent purchases | Retain and deepen loyalty of high-value customers | Provide exclusive previews and early access to new collections.<br>Introduce tiered loyalty rewards to reinforce positive brand experience. |
| **Re-engage** | Previously active customers who have become less engaged | Revive interest and encourage repeat purchases | Use anniversary or upgrade offers.<br>Send personalised product reminders.<br>Highlight affordable items aligned with past purchases to re-spark activity. |
| **Reconnect** | Historically valuable customers who have been inactive for a long time | Reactivate high-value dormant customers | Offer personalised “VIP comeback” campaigns.<br>Provide loyalty reinstatement discounts or exclusive reactivation benefits to remind them of their prior value. |

  <img src="/images/customer_segments.png" alt="Customer Segments" width="80%"/>

  _Bar plots representing number of customers in the segment, and line plots representing the average total monetary spend (in thousands), average frequency of purchases, and recency (in hundreds) of last purchase (smaller value means a more recent purchase)._

## 📦 Page 3: Product — Category and Sub-category Performance

_Snapshot of Dashboard - Product:_


**Key Visuals & Features:**

- Revenue, profit, and quantity sold by category and subcategory (click on category to filter)
- Top 10 products by revenue and profit

**Key Insights:**

- Technology is most profitable despite lowest quantity sold
- Furniture has strong sales but lowest profit
- Certain products have high sales but negative profit (pricing/cost issue)
- Sub-categories with negative profit are: Bookcases, supplies, machines and tables

**Recommended Actions:**

- Maintain stock for high-profit, high-quantity subcategories (binders, paper, accessories, phones)
- Since furnishings have the highest sales volume and generate positive profit, prioritise marketing these products and explore bundling opportunities — for example, pairing chairs with tables.
- Investigate high-sales but low-profit products — renegotiate supplier costs or explore alternatives

## 🧪 Tools Used
- Python: Pandas, Seaborn, Matplotlib, Scikit-Learn
- Tableau: Dashboard creation and visualisation

