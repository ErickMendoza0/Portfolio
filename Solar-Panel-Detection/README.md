# Solar Panel Fault Detection using Deep Learning

## 📌 Project Overview
This project focuses on **Predictive Maintenance** for the energy sector. Using a Convolutional Neural Network (CNN), I developed a model to identify 6 types of conditions in solar panels, aiming to optimize inspection processes using drones (Edge Computing).

## 🛠️ Tech Stack
* **Language:** Python
* **Library:** TensorFlow / Keras
* **Architecture:** MobileNetV2 (Transfer Learning)
* **Dataset:** 6 classes (Clean, Dusty, Bird-drop, Electrical-damage, Physical-Damage, Snow-Covered)

## 📊 Results & Performance
The model was trained using **Data Augmentation** to handle class imbalance.
* **Validation Accuracy:** ~75%
* **Key Finding:** The model excels at detecting "Snow-Covered" and "Dusty" panels but shows areas for improvement in "Physical Damage" due to limited data samples.

### Confusion Matrix
![Confusion Matrix](https://tu-link-de-la-imagen-aqui.png)
*Figure 1: Analysis of true vs. predicted labels showing high precision in environmental factors.*

## 🚀 Engineering Impact
By implementing this model on Edge devices, energy companies can:
1. Reduce maintenance costs by 20-30%.
2. Perform autonomous inspections in remote areas of Ecuador.
3. Prevent permanent cell degradation (Hotspots) caused by partial shading.
