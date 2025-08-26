# Predicción de Consumo Energético en Ecuador

**Objetivo**: Pronosticar consumo energético mensual (2014–2024) y comparar **ARIMA/SARIMA** vs **LSTM/BiLSTM**.

## 📦 Datos
- Fuente: Ministerio de Energía y Minas y la Agencia de Regulación y Control de Electricidad (ARCONEL).
- Frecuencia: Mensual.
- Variables: Consumo [GWh], desagregaciones, etc.

## 🧠 Modelos
- Clásicos: `ARIMA`, `SARIMA` con `statsmodels`.
- Deep Learning: `LSTM`, `BiLSTM` con `TensorFlow/Keras`.

## 🔧 Pipeline
1. Limpieza y tratamiento de valores nulos/outliers.
2. Diferenciación/estacionalidad (modelos clásicos).
3. Ventanas temporales y *feature engineering* (DL).
4. Entrenamiento y validación temporal (*time series split*).
5. Métricas: **RMSE, MAE, MAPE**.

## ▶️ Cómo ejecutar
```bash
pip install -r requirements.txt
jupyter lab
```
Abrir `notebooks/01_eda.ipynb`, `02_modelos_clasicos.ipynb`, `03_lstm.ipynb`.

## 📊 Resultados
- LSTM superó a los modelos estadísticos.
### Comparación de predicciones vs valores reales
A continuación se muestra la serie temporal de consumo energético mensual junto con las predicciones de los modelos estadísticos y de IA.
<<<<<<< HEAD


**ARIMA**
![ARIMA 2014-2023](./resultados/figuras/ARIMA_(2014-2023).png)  
![ARIMA 2014-2024](./resultados/figuras/ARIMA_(2014-2024).png)


**SARIMA**
![SARIMA 2014-2023](./resultados/figuras/SARIMA_(2014-2023).png)  
![SARIMA 2014-2024](./resultados/figuras/SARIMA_(2014-2024).png)


**LSTM**
![LSTM 2014-2023](./resultados/figuras/LSTM_(2014-2023).png)  
![LSTM 2014-2024](./resultados/figuras/LSTM_(2014-2024).png)


**BiLSTM**
![BiLSTM 2014-2023](./resultados/figuras/BiLSTM_(2014-2023).png)  
![BiLSTM 2014-2024](./resultados/figuras/BiLSTM_(2014-2024).png)



### Error por modelo
Comparación de desempeño entre modelos clásicos (ARIMA, SARIMA) y redes neuronales (LSTM, BiLSTM).  
El modelo LSTM logró el mejor resultado, demostrando mayor precisión y adaptabilidad.

| Modelo   | RMSE (GWh) | MAE (GWh) | MAPE (%) |
|----------|------------|-----------|----------|
| ARIMA    | 177        | 155       | 8.63     |
| SARIMA   | 159        | 140       | 7.56     |
| LSTM     | 158        | 143       | 7.80     |
| BiLSTM   | 156        | 143       | 7.75     |

---

### 📌 Conclusiones
- Los modelos basados en **series temporales** (ARIMA y SARIMA) capturan patrones generales, pero muestran mayor error en periodos con alta variabilidad.
- Los modelos **LSTM/BiLSTM** logran capturar dependencias de largo plazo, reduciendo el error promedio.  
- En particular, **LSTM** obtuvo la menor tasa de error, lo que lo posiciona como el modelo más adecuado para este caso de estudio.



## 📁 Estructura sugerida
```
Prediccion_Consumo_Energetico/
├── data/                # (vacío o .gitignored)
├── notebooks/
│   ├── 01_eda.ipynb
│   ├── 02_modelos_clasicos.ipynb
│   └── 03_lstm.ipynb
├── src/
│   ├── preprocessing.py
│   └── utils.py
├── resultados/
│   ├── figuras/
│   └── metricas.json
└── README.md
```
