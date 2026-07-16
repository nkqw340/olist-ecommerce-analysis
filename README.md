# Olist E-Commerce Customer Satisfaction Analysis

## Background
Inspired by Pinduoduo's low-price retention model, this project investigates what actually drives customer satisfaction and repeat purchases on Olist, Brazil's largest e-commerce marketplace.

## Key Findings
- Delivery duration has high relationship with satisfaction. (1-star orders wait 21 days on average vs 5-star orders wait 10 days on average)
- No clear relationship between price and satisfaction, but price may be important possibly as a proxy for product complexity
- Weak correlation between satisfaction and repeat purchases, suggesting Olist is a one-time purchase platform. (Only 3.1% of customers made repeat purchases)
- Olist tends to overestimate delivery timings by 2x

## Project Structure
1. **Data Cleaning** 
   — dtype conversion, null analysis, validity checks
2. **Repeat Purchase Analysis**
   - Does satisfaction drive repeat purchases?
3. **Satisfaction Drivers** — testing three hypotheses:
   - Does price affect satisfaction?
   - Which product categories have the best and worst ratings?
   - Does meeting estimated delivery date predict satisfaction more than speed?
4. **Modelling** 
   — Random Forest vs Logistic Regression to predict satisfaction
   - NLP on review comments to investigate satisfaction factors
5. **SQL Analysis** — key findings reproduced in SQL alongside pandas

## How to Run
1. Download dataset from Kaggle: [https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce?select=olist_order_reviews_dataset.csv]
2. Install requirements: `pip install pandas numpy plotly scikit-learn wordcloud`
3. Open `olist_analysis.ipynb` in Jupyter
4. Run cells sequentially

## Dataset
[Olist Brazilian E-Commerce Dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce?select=olist_order_reviews_dataset.csv) — 100k orders, 2016-2018
