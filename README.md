# 📊 Finance & Investment Analysis – Interview Assessment

### 👤 Author: **Nikhil Dattatray Bamne**
### 🎓 Role: **Senior Finance & Data Analyst (Quantitative Research | Portfolio Optimization | AI & ML in Finance)**
### 🗓️ Prepared For: **Technical & Case-Based Interview Evaluation**

---

## 🧭 Project Overview

This assignment demonstrates end-to-end analytical, financial modeling, and portfolio optimization capabilities across **four key tasks**, each targeting a core competency area in modern finance analytics:

1. **Portfolio Risk & Dashboarding (Visualization)**
2. **Transaction Data & Counterparty Analysis**
3. **Machine Learning for Stock Prediction**
4. **Portfolio Optimization – Mean Variance vs Hierarchical Risk Parity**

Each task simulates a real-world finance use case where quantitative reasoning, Python-based analytics, and visualization merge to produce actionable insights for investment decisions.

---

## 🧩 Task 1: Portfolio Risk & Dashboard

### 🎯 Objective
To design and build a **single-screen Power BI dashboard** that monitors the performance and risk profile of a **hypothetical equally-weighted portfolio** consisting of:
- Fixed Income
- Equity
- Commodity

### 🧠 Approach
- Collected **daily close price data** from the provided worksheets (`Fixed Income`, `Equity`, `Commodity`, and `Benchmark`).
- Computed:
  - **Simple & Log Returns**
  - **Portfolio Daily Return** (equal weighting)
  - **Annualized Return and Volatility**
  - **Sharpe Ratio (Rf = 1%)**
- Generated a **benchmark comparison** to assess portfolio outperformance.
- Built **five Power BI views**:
  1. **Cumulative Return Chart** – Portfolio vs Benchmark
  2. **Rolling Volatility Trend** – 20D Annualized Volatility
  3. **Asset Class Contribution** – Pie/Bar chart for return share
  4. **Correlation Matrix** – Risk diversification view
  5. **Headline Metrics** – Ann. Return, Ann. Vol, Sharpe Ratio

### ⚙️ Tools & Methods
- **Power BI** for visualization and DAX calculations
- **Pandas / NumPy** for pre-processing in Jupyter
- **DAX formulas** for financial metrics (annualized return, volatility)

### 📈 Key Insights
- Equity delivered higher returns but added volatility.
- Commodities acted as a hedge during drawdowns.
- The diversified portfolio achieved a **Sharpe Ratio > 1**, reflecting a balanced risk-reward tradeoff.

---

## 💰 Task 2: Transaction Data – Counterparty Analysis

### 🎯 Objective
Analyze a synthetic transaction dataset to identify **key counterparties and trade patterns** to assist compliance and liquidity risk teams.

### 🧠 Approach
- Loaded transaction-level data using **Pandas**.
- Calculated:
  - **Total transaction value per counterparty**
  - **Top 3 counterparties by exposure**
  - **Trade frequency & average deal size**
- Detected any potential **concentration risk**.
- Exported results to Excel & Power BI visuals for clarity.

### ⚙️ Tools & Methods
- **Python (Pandas, Matplotlib)** for aggregation and summary analysis
- **Power BI** for visualization of top counterparties and exposure ratios

### 📈 Key Insights
- The top 3 counterparties accounted for ~70% of total trade value, suggesting exposure concentration.
- Recommended introducing counterparty caps or internal rating-based limits.

---

## 📉 Task 3: Stock Price Prediction using Machine Learning

### 🎯 Objective
Train and compare predictive models using **Kaggle stock data (train.pkl / test.pkl)** to forecast returns and justify model selection.

### 🧠 Approach
- Data preprocessing:
  - Handled missing values, encoded features, normalized predictors.
- Models evaluated:
  1. **Linear Regression**
  2. **Random Forest Regressor**
  3. **XGBoost Regressor**
- Used **TimeSeriesSplit (5 folds)** for CV.
- Evaluated using **RMSE** and **R² Score**.
- Final model generated predictions for `test.pkl` and saved as `submission.csv`.

### ⚙️ Tools & Libraries
- `pandas`, `scikit-learn`, `xgboost`, `numpy`, `matplotlib`
- Evaluation metric: **Root Mean Square Error (RMSE)**

### 📈 Key Insights
- XGBoost delivered the lowest RMSE and captured nonlinear patterns effectively.
- Linear models underperformed due to regime shifts and feature interactions.
- Demonstrated practical ability to **justify model choice**, not just train models.

---

## ⚖️ Task 4: Portfolio Optimization – MVO vs HRP

### 🎯 Objective
Compare **Mean-Variance Optimization (MVO)** and **Hierarchical Risk Parity (HRP)** frameworks for constructing a diversified US asset portfolio.

### 🧠 Approach
- Selected universe: **US Stocks, Bonds, Commodities** (no raw data provided — simulated with random returns).
- Implemented:
  - **MVO (Markowitz Efficient Frontier)** using `PyPortfolioOpt`
  - **HRP (Hierarchical Risk Parity)** using hierarchical clustering
- Applied practical constraints:
  - Maximum Commodity weight = 20%
  - Target Annual Volatility ≤ 15%

### ⚙️ Tools & Libraries
- `PyPortfolioOpt`, `scipy`, `matplotlib`, `pandas`
- Custom optimization functions to handle real-world portfolio constraints.

### 📊 Results
| Model | Annual Return | Volatility | Sharpe | Key Feature |
|--------|----------------|-------------|---------|--------------|
| **MVO** | Higher Return | Higher Vol | 1.20 | Optimized mathematically |
| **HRP** | Lower Vol | More Stable | 1.05 | Better diversification |

### 🧩 Interpretation
- **MVO** is ideal for return-maximizing investors with risk tolerance.
- **HRP** performs better in uncertain markets by controlling drawdowns.
- Recommended a hybrid approach (HRP-MVO overlay) for central bank reserve portfolios.

---

## 🧰 Tech Stack Summary

| Category | Tools / Libraries |
|-----------|-------------------|
| **Programming** | Python (Pandas, NumPy, Matplotlib, Scikit-Learn, XGBoost) |
| **Portfolio Analytics** | PyPortfolioOpt, Financial Calculations |
| **Visualization** | Power BI, Excel Dashboards |
| **Model Evaluation** | RMSE, Sharpe Ratio, Annualized Volatility |
| **Optimization** | MVO, HRP, Efficient Frontier, Clustering |

---

## 🧠 Interview Talking Points

- Demonstrated integration of **quantitative finance concepts** with **data science techniques**.
- Used **Python for analytics** and **Power BI for communication** – highlighting business storytelling ability.
- Balanced technical accuracy with clarity, aligning with enterprise portfolio management practices.
- Experienced in **asset allocation**, **ML forecasting**, and **data visualization for executive dashboards**.

---

## 📄 Deliverables

| File | Description |
|------|--------------|
| `Interview Questions.xlsx` | Raw data and task instructions |
| `Transaction Data.ipynb` | Jupyter notebook with calculations & plots |
| `stock_timeseries_ml_pipeline.ipynb` | ML model training and evaluation |
| `risk_management_task4.ipynb` | risk management task 4 solution |
| `Risk Dashboard.pbix` | Interactive portfolio risk dashboard |
| `README.md` | Documentation and summary (this file) |

---

## 🏁 Conclusion

This project showcases a **multi-disciplinary finance analyst skill set** — bridging **data analytics, risk management, and quantitative modeling**.
Each task reflects a critical area of real-world financial analytics — from **portfolio monitoring** and **counterparty exposure** to **machine learning forecasting** and **optimization under constraints**.

> 💡 *This demonstrates readiness for data-driven investment analysis, central bank portfolio optimization, and strategic risk reporting roles.*
