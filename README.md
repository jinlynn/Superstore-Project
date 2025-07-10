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
- `superstore_clustering.ipynb` — Notebook for clustering
- `README.md` — This file

## 🧩 Business Question
What are the trends in sales and profitability across products, states, categories and customer segments?

## 📌 Key Performance Indicators (KPIs)
- Total Sales
- Total Profit
- Order Count

## 🖥️ Dashboard Features
- Interactive filter by year
- Trendlines for sales, profit and order volume over time
- Bar charts for performance by product category
- Customer segment breakdown by sales, profit, and customer count
- Most and least profitable consumer states
- Treemap showing sales value (rectangle size) and profit (red = negative, green = positive)

## 💡 Key Insights
- **Customer segments** identified: Nurture, Reward, Re-engage, Reconnect — each with tailored strategies
- Sales, profit and order quantity have been increasing compared to previous years.
- While each year has fluctuations, there is an overall upward trend in sales, profit, and order volume from 2014 to 2017.
- Technology is the most profitable category despite having the fewest orders.
- Furniture generates high sales (comparable to other categories) but delivers significantly lower profit.
- Although there are more 'Nurture' customers than 'Reward' customers, the Reward segment drives more revenue and profit.
- The top 5 most profitable states are: *California, Washington, New York, Delaware, Michigan.*
The least profitable are: *Colorado, Illinois, Tennessee, Pennsylvania, Texas*.
- Some products with high sales have negative profit.
- Some top-selling products are unprofitable, indicating potential issues with pricing, discounting, or fulfilment costs.

## 🔧 Recommended Actions
- Review pricing and discount strategies for Furniture.
- Investigate high-sales, low-profit products as indicated in the treemap.
- Strategies for different customer segments — detailed breakdown of segment definitions and strategic recommendations can be found in `superstore_clustering.ipynb`.
- Reassess operations, services or marketing in low-profit states.

## 🧪 Tools Used
- Python: Pandas, Seaborn, Matplotlib, Scikit-Learn
- Tableau: Dashboard creation and visualisation

