# 📦 Demand Forecasting and Inventory Optimization using Prophet

## 📌 Project Overview

Demand forecasting is a critical component of supply chain management. Accurate demand predictions enable organizations to optimize inventory levels, reduce operational costs, and improve customer satisfaction.

In this project, a time-series forecasting model was developed using **Facebook Prophet** to forecast the demand of the **top-selling product** from the DataCo Supply Chain dataset. Based on the forecasted demand, inventory optimization metrics such as **Safety Stock**, **Reorder Point (ROP)**, and **Economic Order Quantity (EOQ)** were calculated to recommend an optimal inventory policy.

---

## 🎯 Business Problem

Traditional inventory planning often relies on manual estimation and historical intuition, which becomes difficult as businesses grow and demand patterns become increasingly dynamic.

This project addresses this challenge by combining demand forecasting with inventory optimization to support data-driven inventory decisions.

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

## 📈 Model Development

The Prophet forecasting model includes:

- Trend Modeling
- Weekly Seasonality
- Yearly Seasonality
- Indian Public Holidays
- Hyperparameter Tuning
- Cross Validation

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

## 📊 Results

The project successfully:

- Forecasted demand for the next **12 months**
- Evaluated model performance using cross-validation
- Calculated Safety Stock
- Calculated Reorder Point
- Calculated Economic Order Quantity (EOQ)
- Recommended an inventory policy for the top-selling product

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