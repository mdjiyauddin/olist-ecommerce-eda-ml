# Olist E-Commerce Data Analysis (EDA + ML)

Exploratory Data Analysis and a Machine Learning model built on the **Brazilian E-Commerce Public Dataset by Olist** — a real-world, multi-table relational dataset (orders, items, products, customers, payments, reviews).

**Dataset source:** [Kaggle - Olist Brazilian E-Commerce](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

## What this project covers
- Merging 6 relational tables using `order_id` / `customer_id` / `product_id`
- Root-cause analysis of missing values (not treated as random errors)
- Delivery time, order value, category revenue, and state-wise revenue analysis
- Payment behavior analysis
- **Key insight:** Delivery delay has a strong negative relationship with review score — 1-star orders took ~2x longer to deliver than 5-star orders
- A Random Forest Classifier to predict good vs bad reviews, including overfitting diagnosis, class imbalance handling, and permutation-based feature importance validation

## Tools used
`pandas`, `numpy`, `seaborn`, `matplotlib`, `scikit-learn`

## Key Insight
Orders with 1-star reviews took ~21 days on average to deliver, compared to ~10 days for 5-star reviews — delivery speed is one of the strongest drivers of customer satisfaction in this dataset.
