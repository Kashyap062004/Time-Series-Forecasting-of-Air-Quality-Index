# Time Series Forecasting of Air Quality Index (AQI) - Gandhinagar Sector 10

## 📌 Project Overview

This project focuses on time series analysis and forecasting of the **Air Quality Index (AQI)** for **Gandhinagar Sector 10** using both classical statistical models and advanced deep learning techniques. The study aims to provide accurate short-term AQI predictions to support proactive environmental management and public health planning.

---

## 🗃️ Dataset

- **Source**: Central Pollution Control Board (CPCB) [https://airquality.cpcb.gov.in/AQI_India/](https://airquality.cpcb.gov.in/AQI_India/)
- **Timeframe**: May 1, 2019 – February 28, 2025
- **Location**: Gandhinagar, Sector 10
- **Pollutants Tracked**: PM2.5, PM10, NO₂, NH₃, SO₂, CO, O₃

---

## ⚙️ Methodology

### 1. **Data Collection and Preprocessing**
- Data scraped using TypeScript from CPCB's APIs
- Cleaned and structured using Python

### 2. **Exploratory Data Analysis (EDA)**
- Visualization of daily AQI trends
- Stationarity checks via ADF test and rolling statistics
- Time series decomposition (additive and multiplicative)

### 3. **Modeling Approaches**

#### 🔢 Classical Models
- Historical Mean
- Naive Method
- Drift Method
- ARIMA (2,1,1)
- SARIMA (seasonal extension of ARIMA)

#### 🤖 Deep Learning Models
- Recurrent Neural Network (RNN)
- Long Short-Term Memory (LSTM)
- Gated Recurrent Unit (GRU)

#### ⚗️ Hybrid Approach
- **Empirical Mode Decomposition (EMD)** applied to denoise and preprocess the AQI series before feeding it into deep learning models.

---

## 📈 Results Summary

| Model         | RMSE (Test) | MAE (Test) | R² (Test) |
|---------------|-------------|------------|-----------|
| Historical Mean | 22.96     | —          | —         |
| Naive          | 14.28      | —          | —         |
| Drift          | 18.53      | —          | —         |
| ARIMA(2,1,1)   | 4.28       | —          | —         |
| GRU (with EMD) | **9.47**   | **7.55**   | **0.82**  |
| LSTM (with EMD)| 13.36      | 10.92      | 0.64      |
| RNN (with EMD) | 11.90      | 9.71       | 0.71      |

---

## 📂 Project Structure


---

## 🔬 Key Learnings

- ARIMA models perform well for short-term AQI forecasting.
- Deep learning models benefit significantly from preprocessing like EMD.
- GRU with EMD outperforms all other models in terms of accuracy.
- Proper stationarity checks and transformations are crucial in time series modeling.

---

## 🚀 Future Work

- Experiment with **Ensemble EMD (EEMD)**, **VMD**, or **Wavelet Transforms**.
- Incorporate **CNN-LSTM** or **Transformer-based models**.
- Build a **real-time AQI dashboard** for public awareness.

---

## 📜 License

This project is licensed under the [Creative Commons BY 4.0 License](https://creativecommons.org/licenses/by/4.0/).

---

## 👨‍💻 Contributors

- Kashyap Milind Trivedi 
- Akshat Kadia 
- Krishil Jayswal 

---


