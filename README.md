# 📦 Inventory Demand Forecasting & Inventory Optimization using Prophet, ARIMA & SARIMA

An end-to-end Supply Chain Analytics project that forecasts future demand for the top-selling product and converts the forecast into actionable inventory optimization decisions.

The project compares **Prophet**, **ARIMA**, and **SARIMA** forecasting models, performs automatic model selection, validates seasonality using autocorrelation analysis, and recommends inventory policies such as Safety Stock, Reorder Point, and EOQ.

---

## 🎯 Business Problem

Traditional inventory planning often relies on manual estimation and historical intuition, which becomes difficult as businesses grow and demand patterns become increasingly dynamic.

This project addresses this challenge by combining demand forecasting with inventory optimization to support data-driven inventory decisions.

---

---

# 🎯 Project Objectives

- Forecast future demand of the top-selling product.
- Compare Prophet, ARIMA and SARIMA forecasting models.
- Automatically select the best forecasting model.
- Detect seasonality before applying seasonal forecasting.
- Optimize inventory using forecasting results.
- Identify the key factors influencing demand.

---


## ❓ Business Questions Addressed

### 1️⃣ What is the demand forecast for the top-selling product over the next 12 months?

A Prophet time-series forecasting model was developed to predict the future demand of the top-selling product using historical sales data.

### 2️⃣ What is the optimal inventory policy for the top-selling product?

Using the forecasted demand, the following inventory metrics were calculated:

- Safety Stock
- Reorder Point (ROP)
- Economic Order Quantity (EOQ)

These metrics help minimize stockouts while reducing inventory holding and ordering costs.

---
---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Prophet (Facebook Prophet)
- Scikit-learn
- Google Colab

---



---

## 📐 Inventory Optimization Formulas

### 1. Lead Time Demand

```text
Lead Time Demand = Average Daily Demand × Average Lead Time
```

---

### 2. Safety Stock

```text
Safety Stock =
(Maximum Daily Demand × Maximum Lead Time)
−
(Average Daily Demand × Average Lead Time)
```

---

### 3. Reorder Point (ROP)

```text
Reorder Point =
Lead Time Demand + Safety Stock
```

---

### 4. Holding Cost

```text
Holding Cost = 10% × Product Price
```

or

```text
H = 0.10 × Product Price
```

---

### 5. Ordering Cost

```text
Ordering Cost = 30% × Product Price
```

or

```text
S = 0.30 × Product Price
```

---

### 6. Annual Demand

```text
Annual Demand =
Average Daily Forecasted Demand × 365
```

or

```text
D = Average Daily Forecasted Demand × 365
```

---

### 7. Economic Order Quantity (EOQ)

```text
              ___________________
             / 2 × D × S
EOQ = √      -----------
                  H
```

Where:

- **D** = Annual Demand
- **S** = Ordering Cost per Order
- **H** = Holding Cost per Unit per Year

---

# 📉 Visualizations

The notebook includes visualizations for:

- Demand Trend
- Time Series Analysis
- Prophet Forecast
- Forecast Components
- Cross Validation Results
- ACF Plot
- Model Comparison
- Correlation Heatmap
- Feature Importance

---

# 🏆 Key Results

- Successfully forecasted demand for the top-selling product.
- Tuned Prophet model achieved the best forecasting performance.
- Auto ARIMA automatically optimized ARIMA and SARIMA parameters.
- ACF analysis confirmed the absence of statistically significant weekly seasonality.
- SARIMA therefore selected a non-seasonal configuration.
- Forecasts were translated into practical inventory decisions including Safety Stock, Reorder Point, and EOQ.

---

## 💼 Business Impact

The proposed inventory policy can help organizations:

- Reduce stockouts
- Improve product availability
- Minimize inventory holding costs
- Optimize ordering frequency
- Support data-driven inventory planning
- Improve supply chain efficiency

---