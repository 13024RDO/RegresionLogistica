# Predicción de Riesgo Cardíaco con Regresión Logística

Este proyecto aplica un modelo de **Regresión Logística** usando `Scikit-learn` para predecir si un paciente tiene **riesgo de enfermedad cardíaca**, en base a variables clínicas como **edad**, **colesterol** y **presión arterial sistólica**.

---

## Objetivo

Predecir si un paciente presenta **alto riesgo cardíaco (1)** o **bajo riesgo (0)**, ayudando a sistemas de salud a priorizar evaluaciones clínicas con modelos explicables y eficientes.

---

## Dataset

El dataset fue generado de forma **simulada** con lógica médica:
- `edad`: entre 30 y 80 años  
- `colesterol`: entre 150 y 300 mg/dL  
- `presion_sistolica`: entre 100 y 180 mmHg  
- `riesgo_cardiaco`: variable objetivo binaria (0 o 1), determinada mediante una función logística basada en los valores anteriores.

---

## Modelo

Se utiliza `LogisticRegression` de Scikit-learn:

```python
modelo = LogisticRegression()
modelo.fit(X_train, y_train)
