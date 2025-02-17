# Netherlands_Banking_Risk
📊 **Comprehensive Risk Analysis of Dutch & European Banks Using Python**  

This project analyzes financial risk for **Dutch and European banks** using **Value-at-Risk (VaR), Expected Shortfall (ES), Volatility Modeling (GARCH), and Stress Testing**.

## 🏦 Banks Included:
| Country       | Bank Name      |
|--------------|---------------|
| 🇳🇱 Netherlands | NN Group      |
| 🇳🇱 Netherlands | ING Group     |
| 🇳🇱 Netherlands | ABN AMRO      |
| 🇧🇪 Belgium    | KBC Group     |
| 🇩🇪 Germany    | Deutsche Bank |

## 📌 **Project Structure**
This project is structured as follows:
- **Data Collection:** Download stock prices from **Yahoo Finance** (2015-2025).
- **Exploratory Data Analysis (EDA):** Analyzing trends, log returns, and correlations.
- **Risk Analysis:**
  - **Value-at-Risk (VaR)**
  - **Expected Shortfall (ES)**
  - **Stress Testing (COVID-19 Impact)**
- **Predictive Modeling:**
  - **GARCH (Volatility Forecasting)**

---

## 🔹 **Stock Price Trends (2015-2025)**
This visualization tracks the stock price movement of selected banks.

![Stock Price Trends](https://raw.githubusercontent.com/your_username/Netherlands_Banking_Risk/main/Stock_price_trends.png)

### **Key Observations:**
- **KBC Group** had the highest stock price throughout the period.
- **COVID-19 (2020)** caused a sharp decline in all bank stocks.
- **Deutsche Bank** showed strong recovery post-2020.

---

## 🔹 **Log Return Distributions**
This plot displays the **distribution of log returns** for each bank.

![Log Returns](https://raw.githubusercontent.com/your_username/Netherlands_Banking_Risk/main/Distribution_log_returns.png)

### **Key Insights:**
- Most banks show **bell-shaped distributions**, resembling normality.
- **Deutsche Bank & ING Group** exhibit higher volatility with **wider distributions**.

---

## 🔹 **Correlation Matrix**
This heatmap shows **correlations between bank returns**.

![Correlation Matrix](https://raw.githubusercontent.com/your_username/Netherlands_Banking_Risk/main/Correlation_matrix.png)

### **Key Insights:**
- **ABN AMRO & NN Group** have the highest correlation (0.75).
- **Deutsche Bank** is the least correlated with Dutch banks, providing **diversification potential**.

---

## 🔹 **Rolling 30-Day Volatility**
This visualization shows how volatility evolves over time.

![Rolling 30-Day Volatility](https://raw.githubusercontent.com/your_username/Netherlands_Banking_Risk/main/Rolling_30_day_volatility.png)

### **Key Insights:**
- **Volatility spikes in 2020** (COVID-19) and **2022** (economic uncertainties).
- **ING Group** consistently shows higher volatility than others.

---

## 🔹 **Cumulative Log Returns**
This chart shows the **long-term growth performance** of bank stocks.

![Cumulative Log Returns](https://raw.githubusercontent.com/your_username/Netherlands_Banking_Risk/main/Cumulative_Log_Returns.png)

### **Key Insights:**
- **Deutsche Bank** shows the highest **long-term returns**.
- **ING Group performed the worst**, struggling to recover from market downturns.

---

## 🔹 **Value-at-Risk (VaR) Analysis**
We calculate **VaR using three methods**:
1. **Historical VaR** (based on past returns)
2. **Parametric VaR** (Normal distribution assumption)
3. **Monte Carlo VaR** (Simulated losses)

![VaR Analysis](https://raw.githubusercontent.com/your_username/Netherlands_Banking_Risk/main/VaR_Analysis_distribution_of_Returns.png)

| Bank         | Historical VaR | Parametric VaR | Monte Carlo VaR |
|-------------|--------------|---------------|----------------|
| NN Group    | -3.04%       | -3.52%        | -3.56%         |
| ING Group   | -3.87%       | -4.09%        | -4.06%         |
| ABN AMRO    | -2.87%       | -3.39%        | -3.39%         |
| KBC Group   | -2.80%       | -3.23%        | -3.18%         |
| Deutsche Bank | -2.23%     | -2.71%        | -2.68%         |

### **Key Insights:**
- **ING Group** has the highest risk across all VaR models.
- **Deutsche Bank** has the lowest risk.

---

## 🔹 **Expected Shortfall (ES) Analysis**
Expected Shortfall (Conditional VaR) measures **average losses beyond the VaR threshold**.

![Expected Shortfall](https://raw.githubusercontent.com/your_username/Netherlands_Banking_Risk/main/Expected_Shortfall_Analysis.png)

| Bank         | Historical ES | Parametric ES | Monte Carlo ES |
|-------------|--------------|---------------|----------------|
| NN Group    | -5.38%       | -4.41%        | -4.22%         |
| ING Group   | -6.11%       | -5.13%        | -4.22%         |
| ABN AMRO    | -5.04%       | -4.26%        | -4.22%         |
| KBC Group   | -4.83%       | -4.05%        | -4.22%         |
| Deutsche Bank | -4.10%     | -3.40%        | -4.22%         |

### **Key Insights:**
- **ING Group** has the highest Expected Shortfall (~6%).
- **Deutsche Bank** is the most resilient.

---

## 🔹 **COVID-19 Stress Testing**
### **Stock Prices During Crisis**
![Stock Prices COVID-19](https://raw.githubusercontent.com/your_username/Netherlands_Banking_Risk/main/Stock_prices_Covid_19(Feb-Apr_2020).png)

### **Rolling Volatility During Crisis**
![Rolling 10-Day Volatility](https://raw.githubusercontent.com/your_username/Netherlands_Banking_Risk/main/Rolling_10_day_volatility_COVID_19_Crisis.png)

### **Drawdowns During Crisis**
![Drawdown COVID-19](https://raw.githubusercontent.com/your_username/Netherlands_Banking_Risk/main/Drawdown_COVID_19_Crisis.png)

| Bank         | Max Drawdown | Volatility Spike |
|-------------|-------------|------------------|
| NN Group    | -85.8%      | 10.04%           |
| ING Group   | -73.9%      | 8.75%            |
| ABN AMRO    | -91.4%      | 11.12%           |
| KBC Group   | -65.7%      | 10.39%           |
| Deutsche Bank | -62.1%     | 8.77%            |

### **Key Insights:**
- **ABN AMRO was hit the hardest**, with a **91% drop**.
- **Deutsche Bank showed the strongest resilience**.

---

## 🔹 **GARCH Model: Volatility Forecast**
We used **GARCH(1,1) models** to forecast volatility for the next **30 days**.

![GARCH Volatility Forecast](https://raw.githubusercontent.com/your_username/Netherlands_Banking_Risk/main/30-Day_Volatility_Forecast_(GARCH_Model).png)

### **Key Insights:**
- **NN Group’s volatility is declining** (good for stability).
- **ING Group & KBC Group show increasing risk**.

---

## 🚀 **Final Thoughts**
- This project provides **a full risk assessment of European banks**.
- We used **VaR, Expected Shortfall, Stress Testing, and GARCH Forecasting**.
- Future work could include **adding more banks or using machine learning for risk prediction**.

📌 **By Konstantinos Manos**
