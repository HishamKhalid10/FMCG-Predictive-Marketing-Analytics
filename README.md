Data-Driven Business Optimization: Predictive Modeling & Customer Analytics

 Project Overview
An end-to-end data science and Analyist capstone project designed to solve real-world operational and marketing pain points through predictive modeling and unsupervised machine learning. The project is split into two corporate business intelligence tracks:

1. Dynamic Pricing & Demand Forecasting: Built using XGBoost to capture price elasticity and historical seasonality.
2. Customer Behavior Analytics: Built using K-Means Clustering on a 4-month (120-day) operational window to optimize marketing spend.

 Problem Statement & Stakeholder Impact
Pricing Track: Retail management struggles with setting prices without violating economic demand laws. This tracking system enforces negative price elasticity and maps out dynamic financial risk boundaries ($Upper/Lower$ safe bounds) for 2017 inventory planning.
Marketing Track: E-commerce platforms suffer from customer attrition. This track maps a strict 120-day inactive vs. active slicer grid to identify at-risk users and isolate champion cohorts.

 Dataset Descriptions
Sales Data with Dates: Historical transactions with attributes for target prices, categories (`FOODS`, `HOUSEHOLD`, `HOBBIES`), and absolute product quantities.
Olist Brazilian E-commerce Dataset: Multi-table historical data (orders, customers, reviews, items, payments) used to calculate logistics and RFM customer profiles.
Global Ads Performance Dataset: Multi-platform historical advertising records (Meta Ads, Google Ads, TikTok Ads) mapping budget variations to dynamic conversion outcomes.

 Methodology & Technical Framework
Feature Engineering: Extracted dynamic lagging variables (`Lag_1_Month`, `Lag_12_Months`), historical moving averages (`Rolling_Mean_3_Months`), and cyclic seasonality matrices (`Month_Sin`).
Algorithmic Modeling: Trained specialized `XGBoost` and `RandomForestRegressor` models, utilizing validation strategies with strict split evaluations ($R^2$ and $MAE$).
Clustering Architecture: Applied `StandardScaler` transformations to isolate statistical behaviors before executing `K-Means` clustering.

Key Metrics & Model Performance
Price Elasticity Model: Evaluated via strict Mean Absolute Error ($MAE$), yielding real business operational accuracy.
Demand Forecasting Model: Modeled category-specific trends independently using $R^2$ metrics to preserve pure variance data scores.
Advertising Budget Predictor: Leveraged dynamic bin-smoothing to stabilize cross-platform predictive output performance.
