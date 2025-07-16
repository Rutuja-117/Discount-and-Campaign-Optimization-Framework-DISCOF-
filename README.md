# DOCAFE – Discount Optimization and Campaign Forecasting Engine
A machine learning framework that personalizes discount strategies at the user-product level and forecasts campaign outcomes such as GMV, CVR, and Margin. 

Overview-
DOCAFE bridges micro-level personalization and macro-level campaign forecasting in retail analytics.
It combines user behavioral data, transactional logs, and campaign details to:
  -Predict discount thresholds required for individual user-product pairs
  -Forecast key business KPIs like Conversion Rate (CVR), Gross Merchandise Value (GMV), and Margin
  -The framework enables businesses to simulate discount strategies before launch and make data-driven marketing decisions.
  
Data Description-
Enriched_Discount_Dataset.csv — Synthetic dataset with user interactions, discount percentages, demographics, and campaign details.
cleaned_behavior_features.csv — Engineered feature set post-processing.
Note: The dataset used is synthetic, created for experimental validation purposes only.

Models Used-
1. Micro-Model:
Algorithms: Random Forest, XGBoost (final), MLP
Goal: Predict conversion probability & optimal discount
2. Macro-Model:
Algorithms: LSTM, Prophet
Goal: Forecast campaign-level KPIs (CVR, GMV, Margin)

Results Summary-
| Model   | CVR MAPE (%) | GMV MAPE (%) | Margin MAPE (%) |  
|---------|---------------|---------------|------------------|  
| Prophet | **6.9**      | **8.5**           | **9.8**             |  
| LSTM    | **7.8**          | **7.1**       | **6.3**         |  
