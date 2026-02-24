# AXP-Stock-Forecaster-ML
A machine learning pipeline utilizing Ridge Regression to forecast 1-year stock price trajectories based on historical market data.

# 📈 AXP Stock Forecaster ML: 1-Year Stock Predictive Analytics

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)

## 📖 Project Overview
Predicting financial markets is one of the most complex challenges in data science. **AXP Stock Forecaster ML** is an end-to-end machine learning project designed to forecast the closing price of American Express (AXP) stock **one year (252 trading days) into the future**. 

Built with a focus on comprehensive data analysis, this project transforms raw historical market data into engineered features to uncover long-term pricing trends. It serves as a robust baseline for time-series forecasting, bridging the gap between historical financial data and predictive business intelligence.

## ✨ Key Features
* **Time-Series Feature Engineering:** Utilizes critical market indicators, including 50-day and 200-day Moving Averages (MA), alongside daily and cumulative returns.
* **Long-Term Forecasting Horizon:** Employs a `-252` day data shift to train the model specifically for 1-year ahead forecasting, rather than simple next-day predictions.
* **Robust Data Preprocessing:** Implements rigorous train-test splitting (chronological, to prevent data leakage) and feature scaling using `StandardScaler` to normalize high-variance financial figures.
* **Regression Modeling:** Utilizes Ridge Regression (L2 Regularization) to establish a strong, stable mathematical baseline that prevents overfitting on noisy stock data.
* **Performance Evaluation:** Evaluates predictive accuracy using real-world variance metrics: Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE).

## 🛠️ Technology Stack
* **Language:** Python
* **Data Manipulation:** `pandas`, `numpy`
* **Machine Learning:** `scikit-learn` (Ridge Regression, Scalers, Metrics)
* **Visualization:** `matplotlib` (Easily exportable to **Power BI** for executive dashboarding)

## 📊 Visualizing the Forecast
The model outputs a clear comparison between actual historical prices and the 1-year predicted trajectory. 

**Business Intelligence Integration:** The prediction outputs (CSV) are structured to be seamlessly imported into visualization platforms like Power BI. This allows for the creation of professional, KPI-driven financial dashboards (e.g., utilizing a clean blue and grey corporate theme) to present these machine learning insights to stakeholders.

## 🚀 How to Run the Project

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/Priyankghuntala/AXP-Stock-Forecaster-ML.git](https://github.com/Priyankghuntala/AXP-Stock-Forecaster-ML.git)

   Install dependencies:
2. **Install dependencies:**
   ```bash
    pip install pandas numpy scikit-learn matplotlib

3. **Run the predictive model:**
   ```bash
    python model.py


## 🧠 Future Scope & Improvements
While this iteration establishes a strong regression baseline, the volatile nature of the stock market leaves room for advanced iterations:
* Integrating macro-economic variables (Interest Rates, S&P 500 index performance).

* Implementing deep learning architectures such as Long Short-Term Memory (LSTM) networks for sequential pattern recognition.

* Adding sentiment analysis features scraped from financial news APIs.
