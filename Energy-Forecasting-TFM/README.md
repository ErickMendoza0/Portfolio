# Electrical Demand Forecasting: ARIMA vs. LSTM (Master's Thesis)

## 📌 Project Overview
This project is my Master's Thesis, focused on predicting the long-term electrical energy demand in Ecuador. I conducted a comparative study between a classical statistical model (**ARIMA**) and a Deep Learning approach (**LSTM**) to determine which provides better accuracy for national energy planning.

## 📊 Research Results
The study demonstrated that Deep Learning outperforms traditional methods in handling the non-linearities of the Ecuadorian power grid.

* **Best Performing Model:** Long Short-Term Memory (LSTM).
* **Mean Absolute Percentage Error (MAPE):** Achieved a significantly lower error rate compared to ARIMA.
* **Forecast Horizon:** 12-month projections for national energy infrastructure planning.

## 🛠️ Methodology
* **Dataset:** 10 years of historical consumption data from ARCONEL.
* **Feature Engineering:** Time-series decomposition, seasonality analysis, and data normalization.
* **Deep Learning:** Implemented a stacked LSTM architecture using TensorFlow/Keras.

## 📉 Key Visualization
![Forecasting Comparison](https://tu-link-de-la-grafica-tfm.png)
*Figure 1: Comparison of predicted values vs. actual demand, highlighting the LSTM's ability to capture seasonal peaks.*

## 📜 Thesis Document
The full research paper is available in this repository for technical review.
