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
![Comparison of metrics 2023](https://github.com/ErickMendoza0/Portfolio/blob/main/Energy-Forecasting-TFM/Comparacion2023.png?raw=true
)
*Figure 1: Comparison of RMSE and MAE metrics in the 2023 forecast (Normal Conditions).*

![Comparison of metrics 2024](https://github.com/ErickMendoza0/Portfolio/blob/main/Energy-Forecasting-TFM/Comparacion2024.png?raw=true)
*Figure 2: Comparison of RMSE and MAE metrics in the 2024 prediction (Unfavorable conditions due to climatic phenomena)*

![Forecasting Comparison 2023](https://github.com/ErickMendoza0/Portfolio/blob/main/Energy-Forecasting-TFM/Imagen22-LSTM_2023.png?raw=true
)

*Figure 3: Comparison of predicted values ​​vs. actual values ​​of the LSTM 2014-2023 model (Normal Conditions)*

![Forecasting Comparison 2024](https://github.com/ErickMendoza0/Portfolio/blob/main/Energy-Forecasting-TFM/Imagen23-LSTM_2024.png?raw=true
)

*Figure 4: Comparison of predicted values ​​vs. actual values ​​of the LSTM 2014-2024 model (Unfavorable conditions due to climatic phenomena)*

## 📜 Thesis Document
The full research paper is available in this repository for technical review.
