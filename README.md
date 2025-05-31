# 📈 Predicting ETF and Stock Price Trends

This project explores the use of machine learning and statistical models to predict Exchange Traded Fund (ETF) price trends. By leveraging historical price data of top ETFs from 2010 to 2024, we built and compared three predictive models — XGBoost, Prophet, and ARIMA — to assess their forecasting accuracy and applicability in financial decision-making.

---

## 🧠 Objective

To build robust models that predict ETF price movements and provide data-driven insights to guide buy/sell decisions, helping investors mitigate risks and capitalize on opportunities.

---

## 📊 Dataset

- **Source**: [Yahoo Financials Python Library](https://pypi.org/project/yahoofinancials/)
- **Time Period**: Jan 1, 2010 – Mar 1, 2024 (Train), Mar 1, 2024 – Present (Test)
- **Entities**: Top 20 ETFs in the U.S. market
- **Features**: `open`, `high`, `low`, `close`, `volume`, `adj close`, `delta_price`

---

## 🔍 Data Exploration

- **Line plots**: Visualize price trends across ETFs
- **Box plots**: Compare normalized open prices
- **Correlation heatmaps**: Understand inter-feature relationships

---

## 🛠️ Models Used

### 1. **XGBoost**
- Used for high-performance regression
- Tuned with **Optuna** for hyperparameter optimization
- Best performance among the three models

### 2. **Prophet**
- Designed by Facebook for time-series forecasting
- Robust to outliers, captures seasonality

### 3. **ARIMA**
- Traditional statistical model for time series
- Suitable for stationary datasets
- Underperformed in this use case

---

## 🧪 Evaluation Metrics

- **Root Mean Squared Error (RMSE)**
- **Mean Absolute Percentage Error (MAPE)**

| Model     | RMSE   | MAPE    |
|-----------|--------|---------|
| XGBoost   | 6.45   | 1.89%   |
| Prophet   | 44.59  | 9.56%   |
| ARIMA     | 33.05  | 6.24%   |

---

## 🔑 Key Insights

- **XGBoost** outperformed others, capturing short-term momentum using lag features.
- **Day of the Month** and **previous close prices** were top predictors.
- **ETF volatility** correlates with fund ownership levels and market dynamics.
- **ARIMA**, while standard in finance, lacked adaptability in capturing non-linear patterns compared to machine learning models.

---

## 🔮 Future Work

- Try **LSTM** or **ARIMA-GARCH** to better model volatility.
- Combine models (ensemble) for robust forecasting.
- Incorporate macroeconomic indicators (e.g., interest rates, inflation).

---

## 📘 References

- Investopedia, Facebook Prophet, XGBoost Docs, YahooFinance, ETFGI Reports
- Academic papers on ETF impact, price forecasting, and deep learning in finance

---







