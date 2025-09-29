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

## 📌 Key Performance Indicators (KPIs)
Total revenue, profit, number of orders, average order value and their YoY changes.

## 🖥️ Dashboard Features
- Interactive filter by current year and previous year
- 3 tabs/ pages — Home, Regional/ Customer, Product — to provide overall insights and further analysis
- **Home**
    - Trendlines for sales, profit, order volume and average order value over time
    - Revenue, profit and quantity of items sold in each product category (click on category to filter)
    - Top 5 states contributing in revenue, and map of states, coloured by revenue contribution (click on state in map to filter)
    - No. of orders, revenue contribution, and average shipping days for each shipping mode

_Snapshot of Dashboard - Home:_

<img src="/images/Home.png" alt="Snapshot of Dashboard - Home" width="80%"/>

- **Regional/ Customer**
    - Revenue and profit from each customer segment (click on segment to filter)
    - Revenue by states
    - Revenue contribution from each customer cluster (in selected year only)
    - RFM breakdown for each customer cluster (historical)
    - Top 5 states in revenue, profit, and order volume

_Snapshot of Dashboard - Regional/ Customer:_

<img src="/images/Regional_Customer.png" alt="Snapshot of Dashboard - Regional/ Customer" width="80%"/>

- **Product**
    - Revenue, profit and quantity of items sold in each product category (click on category to filter)
    - Revenue, profit and quantity of items sold from each product subcategory, coloured by category
    - Top 10 products in revenue, profit, and quantity of sales

_Snapshot of Dashboard - Product:_

<img src="/images/Product.png" alt="Snapshot of Dashboard - Product" width="80%"/>

## 💡 Key Insights
- Sales, profit and order volume have been increasing compared to previous years.
- Average order value, however, has been declining.
- Customer segment:
    - Consumers contribute the most to revenue and profit.
- Customer clusters identified: Nurture, Reward, Re-engage, Reconnect
    - ‘Reward’, the most valuable customer segment, made up 43% of the customer base in 2017 and contributed 66% of revenue.
    - ‘Nurture’, customers that are considered new to the store, made up 45% of the customer base in 2017 and contributed 29% of revenue.
- States:
    - The top 5 most profitable states are: *California, New York, Washington, Michigan, Georgia.*
    - The top 5 states by revenue are: *California, New York, Washington, Texas, Pennsylvania.*
- Product category:
    - Technology is the most profitable category despite having the fewest quantity sold.
    - Furniture generates high sales (comparable to other categories) but has the lowest profit.
    - Office supplies have sell 3 times more in quantity as they have generally low prices.
- Product sub-category:
    - The top-selling sub-categories are: Phones, chairs, binders, storage, copiers
    - The most profitable sub-categories are: Copiers, accessories, phones, paper, appliances
    - Sub-categories with negative profit are: Bookcases, supplies, machines and tables
- Some products with high sales have negative profit, indicating potential issues with pricing or fulfilment costs.

## 🔧 Recommended Actions
- Focus on the Technology category as they are the highest-selling and most profitable. In particular, the sub-categories copiers, accessories and phones.
- The store should ensure their inventory is well-stocked for items in the top-selling sub-categories: Binders, phones, storage.
- Review pricing and discount strategies for Furniture. Consider cross-selling these low-profit furniture items with best-selling items. For eg., bundle chairs and tables to offset losses.
- Investigate high-sales products with negative profit — consider looking for other suppliers or lower cost alternatives.
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

