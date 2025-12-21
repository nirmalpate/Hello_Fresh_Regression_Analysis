# Hello_Fresh_Regression_Analysis
📈 Marketing Revenue Optimizer: Predictive Analytics & Strategy
📝 Project Overview
This project provides an end-to-end analytical framework for evaluating marketing performance and predicting future revenue. By combining Time Series Decomposition, Statistical Hypothesis Testing, and Machine Learning, we transform raw advertising data into a strategic roadmap for budget allocation and pricing strategy.

💼 Business Context & Strategy
Our goal is to solve the "Marketing Black Box" problem: identifying which dollars spent actually drive incremental growth versus which dollars are simply riding the wave of natural seasonality.

1. The Pricing & "Legacy" Customer Theory
We utilize this framework to test a critical business hypothesis: Does a price decrease lead to sustainable "Legacy" customer growth?

The Insight: Through our Trend Analysis, we distinguish between the "Initial Spike" (immediate reaction to a price drop) and the "New Baseline" (long-term growth).

The Strategy: If the 7-day moving average stabilizes at a higher volume than the pre-drop period, the strategy is deemed a success in building a recurring customer base.

2. Statistical Rigor (ANOVA & T-Tests)
We don't rely on "gut feelings." We use ANOVA to determine if revenue differences between channels (e.g., Google vs. Meta) are statistically significant.

Impact: This prevents "Chasing Noise." If a channel looks better but the P-value is high, we avoid shifting budget to a result that might just be a lucky streak.

🤖 Machine Learning Framework
Regression: Revenue Prediction
We use a Random Forest Regressor to predict daily revenue.

Target: Daily Revenue ($).

Key Drivers: Clicks (70% importance), Spend, and Temporal Seasonality.

Business Value: This allows the finance team to forecast cash flow with an average accuracy of ±$6,833 (MAE).

Classification: High-Performance Identification
Using a Confusion Matrix, we evaluate our ability to predict "High ROAS" days before they happen.

Precision: 82.6% (When we predict a "Win," we are right 8 out of 10 times).

The Confusion Matrix:

True Positives: Successfully identified high-growth opportunities.

False Positives: Identified "False Alarms" where spend was wasted.

📊 Key Performance Visualizations
1. Time Series Decomposition
We break revenue into Trend, Seasonality, and Residuals.

Trend: The true health of the brand.

Seasonality: The "Weekly Heartbeat" (predicting weekend surges).

Residuals: The "Impact of the Unexpected"—this is where we measure the direct effect of specific marketing campaigns or price changes.

2. Feature Importance
This chart reveals the true levers of our business. Our model shows that Clicks (User Intent) are a far stronger predictor of revenue than Impressions (Brand Reach), suggesting our customers are "High-Intent" buyers.

🛠️ Technical Stack
Python 3.x

Pandas/NumPy: Data Orchestration.

Scikit-Learn: Machine Learning (Regression & Classification).

Statsmodels: Time Series Decomposition & Statistical Testing.

Seaborn/Matplotlib: Executive-level data visualization.



🚀 How to Use
Data Prep: Ensure fact_marketing_performance.csv is updated with the latest daily spend and revenue.

Run Analysis: Execute revenue_analysis.py to generate the statistical reports and trend graphs.

ML Training: Run ml_model.py to refresh the Random Forest weights and update the 14-day forecast.
