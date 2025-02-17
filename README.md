# 📊 Netherlands_Banking_Risk 🇳🇱🇧🇪🇩🇪  
🚀 **Comprehensive Risk Analysis of Dutch & European Banks using Python**  
This project conducts **financial risk analysis** on major **Dutch and European banks**, covering **Value-at-Risk (VaR), Expected Shortfall (ES), Stress Testing (COVID-19), and Volatility Forecasting (GARCH)**.

---

## 🔍 **Project Overview**
This project explores **stock market risk** for five major banks across the Netherlands, Belgium, and Germany:  
✅ **NN Group (Netherlands)**  
✅ **ING Group (Netherlands)**  
✅ **ABN AMRO (Netherlands)**  
✅ **KBC Group (Belgium)**  
✅ **Deutsche Bank (Germany)**  

📌 **[Check the full analysis in the Jupyter Notebook](./Risk_Analysis.ipynb)**  

---

## 📂 **Project Structure**


---

## 📜 **Jupyter Notebooks Overview**
### 1️⃣ **Download & Clean Dataset**  
📌 **[download_clean_dataset.ipynb](./download_clean_dataset.ipynb)**  
- Fetches stock price data from **Yahoo Finance**.  
- Cleans missing values using **forward-fill and back-fill methods**.  
- Saves the **clean dataset** for further analysis.  

---

### 2️⃣ **Exploratory Data Analysis (EDA)**  
📌 **[EDA.ipynb](./EDA.ipynb)**  
- **Stock Price Trends Analysis** (2015-2025).  
- **Log Return Distributions** to assess risk exposure.  
- **Correlation Matrix** to examine interdependencies.  
- **Rolling 30-Day Volatility Trends** to analyze risk fluctuations.  

📊 **Stock Price Trends:**  
![Stock Price Trends](https://raw.githubusercontent.com/your_username/Netherlands_Banking_Risk/main/Images/Stock_price_trends.png)

📊 **Correlation Matrix:**  
![Correlation Matrix](https://raw.githubusercontent.com/your_username/Netherlands_Banking_Risk/main/Images/Correlation_matrix.png)

📊 **Rolling 30-Day Volatility:**  
![Rolling 30-Day Volatility](https://raw.githubusercontent.com/your_username/Netherlands_Banking_Risk/main/Images/Rolling_30_day_volatility.png)

---

### 3️⃣ **Risk Analysis: VaR & Expected Shortfall**  
📌 **[Risk_Analysis.ipynb](./Risk_Analysis.ipynb)**  
- **Value-at-Risk (VaR)**  
  - **Historical VaR**  
  - **Parametric VaR (Variance-Covariance method)**  
  - **Monte Carlo VaR**  

📊 **VaR Distribution Analysis:**  
![VaR Analysis](https://raw.githubusercontent.com/your_username/Netherlands_Banking_Risk/main/Images/VaR_Analysis_distribution_of_Returns.png)

- **Expected Shortfall (ES) Calculation**  
📊 **Expected Shortfall (ES) Analysis:**  
![Expected Shortfall](https://raw.githubusercontent.com/your_username/Netherlands_Banking_Risk/main/Images/Expected_Shortfall_Analysis.png)

---

### 4️⃣ **Stress Testing: COVID-19 Market Impact**  
📌 **[Risk_Analysis.ipynb](./Risk_Analysis.ipynb) – Stress Testing Section**  
We analyzed how the COVID-19 crisis impacted these banks:  

📊 **Stock Prices During Crisis:**  
![Stock Prices COVID-19](https://raw.githubusercontent.com/your_username/Netherlands_Banking_Risk/main/Images/Stock_prices_Covid_19(Feb-Apr_2020).png)

📊 **Volatility Spikes During Crisis:**  
![Rolling Volatility](https://raw.githubusercontent.com/your_username/Netherlands_Banking_Risk/main/Images/Rolling_10_day_volatility_COVID_19_Crisis.png)

📊 **Drawdown Analysis:**  
![Drawdown COVID-19](https://raw.githubusercontent.com/your_username/Netherlands_Banking_Risk/main/Images/Drawdown_COVID_19_Crisis.png)

| Bank         | Max Drawdown | Volatility Spike |
|-------------|-------------|------------------|
| NN Group    | -85.8%      | 10.04%           |
| ING Group   | -73.9%      | 8.75%            |
| ABN AMRO    | -91.4%      | 11.12%           |
| KBC Group   | -65.7%      | 10.39%           |
| Deutsche Bank | -62.1%     | 8.77%            |

---

### 5️⃣ **Predictive Risk Modeling: GARCH Volatility Forecast**  
📌 **[GARCH(1,1).ipynb](./GARCH(1,1).ipynb)**  
We use **GARCH(1,1) models** to forecast future volatility for banks.

📊 **30-Day Volatility Forecast:**  
![GARCH Forecast](https://raw.githubusercontent.com/your_username/Netherlands_Banking_Risk/main/Images/30-Day_Volatility_Forecast_(GARCH_Model).png)

**Key Findings:**  
- **NN Group’s volatility is declining** (stabilizing).  
- **ING Group & KBC Group are expected to become riskier**.  
- **ABN AMRO & Deutsche Bank have the lowest forecasted volatility**.  

---

## 🛠 **Technologies Used**
- **Python**: Pandas, Statsmodels, Matplotlib, Seaborn  
- **Risk Modeling**: VaR, Expected Shortfall, Monte Carlo Simulations  
- **Time Series Forecasting**: GARCH Model for volatility prediction  
- **Data Visualization**: Matplotlib & Seaborn  

---

## 🚀 **Final Thoughts**
✅ This project provides a **full risk assessment** of European banks.  
✅ We used **VaR, Expected Shortfall, Stress Testing, and GARCH Forecasting**.  
✅ Future improvements could include:  
📌 **Expanding the dataset to include more European banks**.  
📌 **Using Machine Learning models for risk classification**.  
📌 **Backtesting trading strategies using our VaR models**.  

---

📌 **By Konstantinos Manos**
