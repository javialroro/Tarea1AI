# 📘 Tarea 02: Implementación de Regresión Lineal con Descenso de Gradiente  

**Curso:** Inteligencia Artificial  
**Escuela:** Ingeniería en Computación  
**Profesor:** Steven Andrey Pacheco Portuguez  
**Instituto Tecnológico de Costa Rica** 

---

## 🎯 Objetivo
El propósito de esta tarea es **implementar y analizar un modelo de regresión lineal desde cero**, utilizando únicamente **NumPy** y **Pandas**.  
El modelo se aplicará al dataset [Student Performance Prediction (Kaggle)](https://www.kaggle.com/datasets/nikhil7280/student-performance-multiple-linear-regression/data) y se evaluará su desempeño mediante métricas implementadas manualmente.  

---

## 📝 Contenido del Proyecto

### 1️⃣ Descarga y Lectura del Dataset
- Carga del dataset en un DataFrame con **Pandas**.  
- Exploración de filas, columnas y tipos de variables.  
- Estadísticas descriptivas (media, desviación estándar, mínimo, máximo).  

### 2️⃣ Análisis Exploratorio de Datos (EDA)
- Histogramas y boxplots de variables numéricas.  
- Diagramas de dispersión entre características y la variable objetivo.  
- Matriz de correlación con mapa de calor.  
- Identificación y tratamiento de **outliers** (si existen).  
- Interpretación de resultados más allá de las visualizaciones.  

### 3️⃣ División del Dataset
Implementación manual de:
- **Muestreo aleatorio (Random Sampling).**  
- **Muestreo estratificado (Stratified Sampling).**  

📌 División:  
- 70% Entrenamiento  
- 15% Validación  
- 15% Prueba  

> ⚠️ No se permite usar `train_test_split` de Scikit-learn.  

### 4️⃣ Implementación de Regresión Lineal
- Implementación de **Batch Gradient Descent** con NumPy.  
- Actualización manual de parámetros:  

  θ := θ - α · ∇L(θ)

- Opción de **Mini-Batch Gradient Descent** como extra.  

### 5️⃣ Evaluación del Modelo
- Cálculo manual del **Error Cuadrático Medio (MSE)**.  
- Visualización de la evolución del MSE en entrenamiento y validación.  
- Comparación entre **training vs validation** para detectar overfitting.  

### 6️⃣ Análisis de Resultados
- Evaluación final con el conjunto de prueba.  
- Gráfico de **residuos vs predicciones**.  
- Discusión e interpretación de los resultados obtenidos.  

---

## 📂 Entregables
La entrega final consiste en un archivo `.zip` con:  
- 📄 **Informe en LaTeX (IEEE Template).**  
- 📑 **PDF del informe.**  
- 📓 **Jupyter Notebook con el código implementado.**  

---

## 🚀 Tecnologías Utilizadas
- Python 3  
- NumPy  
- Pandas  
- Matplotlib (para visualización)  
- Jupyter Notebook  
- LaTeX (Overleaf, plantilla IEEE)  

---

## 👥 Autores

[![GitHub - javialroro](https://img.shields.io/badge/GitHub-javialroro-blue?logo=github)](https://github.com/javialroro)  
[![GitHub - usuario1](https://img.shields.io/badge/GitHub-emmasae01-blue?logo=github)](https://github.com/emmasae01)  
[![GitHub - usuario2](https://img.shields.io/badge/GitHub-Drio02-blue?logo=github)](https://github.com/Drio02)  

📅 **Año:** 2025  
