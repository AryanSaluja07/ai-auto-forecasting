AI-Powered Automobile Sales Forecasting & Business Intelligence Dashboard
End-to-End Business Analyst Project using Python, XGBoost, SHAP Explainability & Power BI

This project builds a complete automobile sales forecasting system using machine learning, enhances trust with explainable AI (SHAP), and communicates insights using a professional Power BI dashboard with a conceptual AI Sales Advisor.

It demonstrates skills across:

Business analysis

Data analysis & preparation

Forecast modeling (XGBoost)

Explainable AI

Power BI dashboarding

Product thinking

📌 Project Overview

Automobile manufacturers and dealerships need accurate demand forecasts to support:

Inventory planning

Supply chain management

Pricing strategy

Branch performance monitoring

Model-level product decisions

This project solves the problem by:

✔ Building a forecasting model using XGBoost
✔ Engineering date-based features for seasonality
✔ Using SHAP to explain predictions
✔ Designing a Power BI dashboard for stakeholders
✔ Adding an AI Sales Advisor concept for conversational analytics

📂 Project Structure
ai-auto-forecasting/
│
├── data/
│   ├── car_sales_clean.csv
│   ├── xgb_time_forecasts.csv
│   └── dashboard_dataset.csv
│
├── notebooks/
│   ├── 01_eda.ipynb
│   ├── 02_forecasting.ipynb
│   └── 03_shap_explainability.ipynb
│
├── reports/
│   ├── shap_bar.png
│   ├── shap_beeswarm.png
│   └── dashboard_screenshots/
│
├── src/
│   ├── data_prep.py
│   ├── xgb_training.py
│   └── utils.py
│
└── README.md

🔍 Phase 1 — Business Understanding
Business Challenge

Dealerships must forecast monthly demand across branches and models to avoid:

Overstocking (increased holding cost)

Stockouts (lost sales)

Poor pricing decisions

Underperforming branches

Project Goals

Predict monthly units sold

Understand the biggest demand drivers

Visualize results clearly

Add a conversational AI concept for modern analytics

📊 Phase 2 — EDA & Data Preparation

Key steps:

Checked missing values and outliers

Explored trends in pricing, models, and branches

Analyzed monthly/seasonal patterns

Created date-based features:

year
month
month_sin  → captures cyclical yearly patterns
month_cos  → improves seasonality modeling


One-hot encoded branch and model

🤖 Phase 3 — Forecast Model (XGBoost)
Why XGBoost?

Handles non-linearity

Works well with engineered features

Fast & reliable for tabular data

Features used:
year
month
month_sin
month_cos
avg_price
branch_* (one-hot)
model_* (one-hot)


The model predicts:

units_sold

Outputs:

✔ 3-Month ahead forecast saved as
xgb_time_forecasts.csv

🧠 Phase 4 — Explainability with SHAP

SHAP is used to:

Identify top global drivers of sales

Understand feature influence direction

Explain individual predictions (local explanations)

Key Findings:

avg_price strongly impacts units sold

Higher price → lower demand

Seasonality exists

Some models consistently outperform

Certain branches have significantly higher sales

SHAP reveals the reasoning behind every prediction

Included plots:

shap_bar.png

shap_beeswarm.png

📈 Phase 5 — Power BI Dashboard
Dashboard Contains:
1. KPI Cards

Total Units Sold (Historical)

Predicted Units Next Month

2. Trends

Sales Over Time (Historical vs Forecast)

Average Price Trend

3. Performance Breakdown

Units Sold by Branch

Units Sold by Model

4. Explainable AI Section

SHAP Global Importance

SHAP Beeswarm Summary

5. AI Sales Advisor Panel (Concept)

A conceptual natural-language interface where users could ask:

• Which branches are expected to grow next month?
• Forecast demand for [Model] for the next 3 months.
• Which models are most price-sensitive?
• Why did sales drop in February?
• What affects sales the most?


This demonstrates LLM integration thinking and real-world BI usage.

💡 Key Business Insights

Ford and Dodge branches dominate sales

F-Series, Explorer, and Camry are high-demand models

Price sensitivity is strong — lower prices correlate with higher sales

Seasonal patterns influence demand

Branch productivity varies significantly

SHAP analysis validates model trustworthiness

🛠 Technologies Used
Category	Tools
Language	Python
ML Model	XGBoost
Explainability	SHAP
Visualization	Power BI
Dev Tools	Git, GitHub
Data Processing	Pandas, NumPy
Notebooks	Jupyter

Future Enhancements

Live API deployment of model

Real LLM chatbot using OpenAI API

Automated data pipeline (Airflow)

Branch-level inventory optimization

Anomaly detection for sudden sales spikes/drops

👤 Author

Aryan Saluja
Business Analyst • Data Analyst • AI Enthusiast
🔗 [Aryan Saluja LinkedIN](https://www.linkedin.com/feed/)