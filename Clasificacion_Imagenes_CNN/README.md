# Clasificación de Imágenes con CNN

**Objetivo**: Clasificar imágenes (p.ej., satelitales o fenómenos naturales) con **transfer learning** y **data augmentation**.

## 🧠 Arquitectura
- *Backbones* sugeridos: `MobileNetV2`, `ResNet50`, `EfficientNetB0`.
- *Callbacks*: *EarlyStopping*, *ReduceLROnPlateau*, *ModelCheckpoint*.

## ▶️ Cómo ejecutar
```bash
pip install -r requirements.txt
jupyter lab
```
Configura `DATA_DIR` en el notebook. Incluye instrucciones para descargar el dataset.

## 📈 Resultados esperados
- *Accuracy* de validación **> 90%** (según dataset).
- Matriz de confusión y clasificación.
