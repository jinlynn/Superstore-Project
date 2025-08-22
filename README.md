# 🛒 Customer Segmentation & Sales Analysis: Superstore Dataset

## 📌 Project Overview
A customer segmentation and sales analysis project using the Superstore dataset from Kaggle ([link](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final/data)). The dataset contains with 9,994 transactions from 2014 to 2017. It includes information on sales, profit, orders, products, states, and customer details.

The project combines unsupervised clustering and an interactive dashboard to derive actionable insights for business strategy.

🔗 **Interactive Dashboard**: [View on Tableau Public](https://public.tableau.com/shared/KN6CQQS28?:display_count=n&:origin=viz_share_link)

## 🎯 Objectives
- Segment customers based on recency, frequency and monetary value.
- Recommend tailored strategies for each customer segment.
- Analyse trends in sales and profitability across products, categories, states, and segments.

## 📁 Files and Structure
- images — Visuals used in the README
- `superstore_clustering.ipynb` — Notebook for clustering
- `README.md` — Project overview and documentation

## 🧩 Business Questions
- Which product category is the best selling and most profitable?
- Which customer segment is bringing in the most revenue and is the most profitable?
- Which state is the most profitable?
- What are their best-selling products?

## 📌 Key Performance Indicators (KPIs)
- Total Sales
- Total Profit
- Order Count

## 🖥️ Dashboard Features
- Interactive filter by year
- Trendlines for sales, profit and order volume over time
- Bar charts for performance by product category (orange diamond represents value in previous year)
- Customer segment breakdown. Hovering the cursor over a rectangle will reveal the number of customers in the segment, and its sales and profit for the year.
- Most and least profitable consumer states
- Treemap showing sales value (rectangle size) and profit (red = negative, green = positive). Hovering the cursor over a rectangle will reveal the name of item, its category, and its sales and profit for the year.

  <img src="/images/dashboard_preview.png" alt="Snapshot of Dashboard" width="80%"/>

_Snapshot of Sales Dashboard._

## 💡 Key Insights
- Sales, profit and order quantity have been increasing compared to previous years.
- While each year has fluctuations, there is an overall upward trend in sales, profit, and order volume from 2014 to 2017.
- Product category:
    - Technology is the most profitable category despite having the fewest orders.
    - Furniture generates high sales (comparable to other categories) but has the lowest profit.
    - Office supplies have the most orders as they have generally low prices.
- Product sub-category:
    - The top-selling sub-categories are: Phones, chairs, binders, storage, copiers
    - The most profitable sub-categories are: Copiers, accessories, phones, paper, appliances
    - Sub-categories with negative profit are: Bookcases, supplies, machines and tables
    - The sub-categories with the most orders are: Binders, paper, furnishings, phones and storage
- Customer segments identified: Nurture, Reward, Re-engage, Reconnect
    - ‘Reward’, the most valuable customer segment, made up 37% of the customer base in 2017 and contributed 66% of revenue.
    - ‘Nurture’, customers that are considered new to the store, made up 40% of the customer base in 2017 and contributed 30% of revenue.
- States:
    - The top 5 most profitable states are: *California, Washington, New York, Delaware, Michigan.*
    - The least profitable are: *Colorado, Illinois, Tennessee, Pennsylvania, Texas*.
- Some products with high sales have negative profit, indicating potential issues with pricing, discounting, or fulfilment costs.

## 🔧 Recommended Actions
- Focus on the Technology category as they are the highest-selling and most profitable. In particular, the sub-categories phones, accessories and copiers.
- The store should ensure their inventory is well-stocked for items in the top-selling and most-orders sub-categories: Binders, phones, storage
- Review pricing and discount strategies for Furniture. Consider cross-selling these low-profit furniture items with best-selling items. For eg., bundle chairs and tables to offset losses.
- Investigate high-sales, low-profit products as indicated in the treemap — consider looking for other suppliers or lower cost alternatives.
- Reassess operations, services or marketing in low-profit states.
- Strategies for different customer segments

  <img src="/images/customer_segments.png" alt="Customer Segments" width="80%"/>

  _Bar plots representing number of customers in the segment, and line plots representing the average total monetary spend (in thousands), average frequency of purchases, and recency (in hundreds) of last purchase (smaller value means a more recent purchase)._
  - **Nurture**: This group consists of new, low-value, and infrequent buyers who have made only small or one-time purchases. Their limited interaction suggests low familiarity with the brand, and they may be unsure about the value or fit of the products. To build trust and encourage continued engagement, offer a limited-time discount on their next purchase to prompt immediate action. Use targeted product recommendations, such as “frequently bought together” items, to reduce decision fatigue and increase cart size. Additionally, introduce a referral rewards program that incentivises them to share the brand with friends — for example, offering a discount when a referred friend makes a purchase. This both grows the customer base and reinforces brand trust.
  - **Reward**: These are high-value buyers who show average recency, above-average frequency, and high monetary value. They’ve demonstrated strong engagement and brand preference by purchasing recently and repeatedly. To retain this valuable group, focus on rewarding their loyalty with meaningful, experience-driven benefits. Offer perks such as exclusive product previews, early access to new collections, or tiered loyalty rewards that recognise their continued support. These actions reinforce their positive experience with the brand, keeping them both satisfied and engaged.
  - **Re-engage**: This segment includes customers with high recency, average frequency, but lower-than-average spend. These are older buyers who have lapsed in value, and may be losing interest or shifting attention to competitors. The goal is to bring them back into the purchase cycle through gentle nudges and smart incentives. Consider anniversary discounts, product upgrade reminders, or targeted low-cost recommendations tailored to their previous purchases. Personalised emails featuring popular, affordable items they might like can reduce friction and make re-engagement more approachable and effective.
  - **Reconnect**: This group consists of old customers with high historical spend. Though they haven’t purchased in a long time, their previous transactions indicate significant value. Appeal to their sense of exclusivity by offering membership-based incentives — for example, “Spend again to keep your VIP status” or a one-time loyalty discount. These customers may not respond to generic campaigns, but a personalised reminder of the value they once saw in the brand can motivate a return.

## 🧪 Tools Used
- Python: Pandas, Seaborn, Matplotlib, Scikit-Learn
- Tableau: Dashboard creation and visualisation

