# Predicción de la velocidad de corrosión en aceros inoxidables mediante Machine Learning

## Proyecto Final - Talento Tech

**Autora:** Irene Rendón

---

# Descripción

Este proyecto desarrolla un modelo de **Machine Learning** para predecir la **velocidad de corrosión** de diferentes familias de **aceros inoxidables**, utilizando información ambiental, química y metalúrgica proveniente del dataset **CORR-DATA**.

Se implementó un flujo completo de Ciencia de Datos que incluye:

- Selección del dataset.
- Análisis exploratorio (EDA).
- Limpieza y preparación de datos.
- Transformación de variables.
- Entrenamiento de modelos de regresión.
- Evaluación mediante métricas.
- Validación cruzada.
- Interpretación de variables importantes.

---

# Objetivo

Analizar qué factores influyen en la velocidad de corrosión de los aceros inoxidables y desarrollar un modelo capaz de estimar dicha velocidad utilizando técnicas de Machine Learning.

---

# Dataset

**Nombre:**

CORR-DATA Database

**Origen:**

National Institute of Standards and Technology (NIST)

En este repositorio se incluye una copia del dataset utilizado.

📄 **Descargar dataset**

[CORR-DATA_Database.csv](./CORR-DATA_Database.csv)

---

# Variables utilizadas

Entre las principales variables empleadas se encuentran:

- Environment
- Material Family
- Material
- Concentration (Vol %)
- Temperature (deg C)
- Duration
- Localized Attack
- Rate (mm/yr) or Rating (variable objetivo)

---

# Tecnologías utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-Learn
- Google Colab

---

# Modelos implementados

Se entrenaron dos modelos de regresión:

- Regresión Lineal
- Random Forest Regressor

Posteriormente se comparó su desempeño utilizando distintas métricas.

---

# Resultados

El modelo **Random Forest** obtuvo el mejor desempeño.

Métricas obtenidas:

|Modelo|MAE|RMSE|R²|
|------|------:|------:|------:|
|Regresión Lineal|0.809|2.442|0.098|
|Random Forest|0.458|1.875|0.468|

Además se realizó una **Validación Cruzada (5-Fold Cross Validation)** para evaluar la capacidad de generalización del modelo.

---

# Principales hallazgos

Las variables con mayor importancia durante la predicción fueron:

- Concentración del medio
- Tiempo de exposición
- Temperatura
- Tipo de acero inoxidable
- Ambiente corrosivo
- Ataque localizado

Los resultados obtenidos son consistentes con los fundamentos de la ingeniería de materiales y la corrosión.

---

# Cómo ejecutar el proyecto

1. Clonar este repositorio.

```bash
git clone https://github.com/TU_USUARIO/Entrega_Final_Machine_Learning.git
```

2. Abrir el notebook **Proyecto_Final_Machine_Learning.ipynb**

3. Instalar las librerías necesarias:

```bash
pip install pandas numpy matplotlib scikit-learn
```

4. Ejecutar todas las celdas del notebook.

---

# Estructura del proyecto

```
Entrega_Final_Machine_Learning
│
├── Proyecto_Final_Machine_Learning.ipynb
├── CORR-DATA_Database.csv
├── README.md
└── img
```

---

# Conclusiones

El modelo desarrollado demuestra que es posible utilizar técnicas de Machine Learning para estimar la velocidad de corrosión de aceros inoxidables a partir de variables ambientales y metalúrgicas.

El algoritmo Random Forest obtuvo el mejor desempeño y permitió identificar los factores con mayor influencia en la predicción, aportando información útil para el análisis del fenómeno de corrosión.

---

# Autor

**Irene Rendón**

Proyecto Final — Talento Tech

2026
