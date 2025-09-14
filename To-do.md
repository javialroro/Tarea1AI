# ✅ To-Do List – Proyecto Student Performance

## 📂 Lectura del Dataset
- [ x] Cargar el dataset con Pandas  
  - [ x] `pd.read_csv("Student_Performance.csv")`  
  - [ x] Guardar en un DataFrame llamado `df`.
- [ ] Explorar estructura del dataset  
  - [ x] Revisar filas y columnas → `df.shape`  
  - [ x] Ver columnas y tipos de datos → `df.info()`  
- [ X] Revisar calidad básica  
  - [ X] Verificar nulos → `df.isna().sum()`  
  - [ X] Detectar duplicados → `df.duplicated().sum()`
- [ ] Obtener estadísticas descriptivas  
  - [ X] `df.describe()` → mean, std, min, cuartiles, max  
  - [ X] `df.describe(include='all')` para incluir categóricas
- [ ] Interpretar resultados  
  - [ ] Confirmar tipos de datos correctos  
  - [ ] Identificar rangos de valores  
  - [ ] Decidir tratamiento de duplicados  
  - [ ] Concluir si el dataset está limpio o si requiere ajustes  

---

## 🔍 EDA (Exploratory Data Analysis)
- [ ] Histogramas y Boxplots  
  - [ ] Generar histogramas de variables numéricas  
  - [ ] Generar boxplots de esas variables  
  - [ ] Interpretar distribuciones y outliers
- [ ] Diagramas de dispersión (vs target)  
  - [ ] Hacer scatter plots contra *Performance Index*  
  - [ ] Interpretar relaciones lineales/no lineales y outliers
- [ ] Matriz de correlación (heatmap)  
  - [ ] Calcular correlaciones  
  - [ ] Visualizar con mapa de calor  
  - [ ] Interpretar correlaciones fuertes y colinealidades
- [ ] Detección y tratamiento de outliers  
  - [ ] Revisar boxplots  
  - [ ] Decidir mantener, winsorizar o eliminar  
  - [ ] Documentar decisión
- [ ] Interpretación global  
  - [ ] Identificar variables más importantes  
  - [ ] Concluir sobre outliers, distribuciones y posibles transformaciones  

---

## ✂️ División del Dataset
- [ x] Preparación  
  - [ x] Definir `X` (features) y `y` (target)  
  - [ x] Convertir categóricas a numéricas  
  - [x ] Preparar funciones para escalado  
  - [ x] Añadir columna de 1’s (bias)
- [ x] Muestreo aleatorio (70/15/15)  
  - [ X] Barajar índices  
  - [ X] Generar splits `train/val/test`  
  - [x ] Escalar con estadísticas del train
- [x ] Muestreo estratificado  
  - [ x] Binear *Performance Index*  
  - [ x] Dividir cada estrato en 70/15/15  
  - [ x] Escalar igual que aleatorio  
  - [ x] Añadir bias
- [ ] Validación de particiones  
  - [ ] Revisar tamaños de splits  
  - [ ] Comparar distribuciones de *Performance Index*  
- [ ] Documentación  
  - [ ] Tabla/figura comparando aleatorio vs estratificado  
  - [ ] Justificar elección  

---

## 📈 Implementación de Regresión Lineal
- [ ] Preparación de datos  
  - [ ] Confirmar target y features  
  - [ ] Codificar categóricas  
  - [ ] Dividir en train/val/test  
  - [ ] Escalar con train  
  - [ ] Añadir bias  
  - [ ] Fijar semilla
- [ ] Definiciones matemáticas  
  - [ ] Hipótesis: ŷ = Xθ  
  - [ ] Costo: MSE  
  - [ ] Gradiente: ∇θL = (2/m)·Xᵀ(Xθ − y)
- [ ] Inicialización e hiperparámetros  
  - [ ] Inicializar θ  
  - [ ] Seleccionar learning rate α  
  - [ ] Definir número de épocas  
  - [ ] (Opcional) Regularización L2  
- [ ] Batch Gradient Descent  
  - [ ] Forward pass  
  - [ ] Calcular gradiente  
  - [ ] Actualizar θ  
  - [ ] Registrar MSE (train/val)  
  - [ ] Proteger contra errores numéricos
- [ ] Monitoreo y parada  
  - [ ] Graficar pérdidas train vs val  
  - [ ] Implementar early stopping (opcional)  
  - [ ] Guardar mejor θ
- [ ] Evaluación final  
  - [ ] Predecir en test  
  - [ ] Calcular MSE y R²  
  - [ ] Graficar residuos vs predicciones  
  - [ ] Guardar artefactos (`theta.csv`, métricas, historial)
- [ ] Mini-Batch Gradient Descent (opcional)  
  - [ ] Definir batch_size  
  - [ ] Implementar mini-batch loop  
  - [ ] Comparar convergencia vs batch
- [ ] Experimentos y reporte  
  - [ ] Búsqueda de hiperparámetros  
  - [ ] Comparar splits aleatorio vs estratificado  
  - [ ] Redactar conclusiones  

---

## 📊 Evaluación del Modelo
- [ ] Definir métricas  
  - [ ] Implementar MSE manualmente  
  - [ ] (Opcional) Implementar R²
- [ ] Calcular durante el entrenamiento  
  - [ ] MSE en train y val  
  - [ ] Guardar historial
- [ ] Visualización  
  - [ ] Graficar curva de pérdidas (train vs val)  
  - [ ] Añadir título, ejes, leyenda
- [ ] Evaluación final en test  
  - [ ] Calcular MSE en test  
  - [ ] Guardar en CSV
- [ ] Análisis e interpretación  
  - [ ] Comparar train vs val  
  - [ ] Evaluar overfitting/underfitting  
  - [ ] Comparar aleatorio vs estratificado  
- [ ] Entregables  
  - [ ] Curva de pérdidas  
  - [ ] MSE en test  
  - [ ] Interpretación escrita  
  - [ ] Archivos en `/results`

---

## 🔮 Análisis Final
- [ ] Predicciones en test  
  - [ ] Calcular ŷ_test = X_test θ  
  - [ ] Comparar con y_test
- [ ] Métrica final  
  - [ ] Reportar MSE  
  - [ ] (Opcional) Reportar R²
- [ ] Gráfico de residuos  
  - [ ] X = predicciones, Y = residuos  
  - [ ] Línea en 0  
  - [ ] Analizar dispersión y outliers
- [ ] Interpretación  
  - [ ] Revisar residuos centrados en 0  
  - [ ] Detectar heterocedasticidad  
  - [ ] Evaluar ajuste lineal
- [ ] Comparación de splits  
  - [ ] Evaluar diferencias entre aleatorio y estratificado
- [ ] Síntesis  
  - [ ] Evaluar si regresión lineal es suficiente  
  - [ ] Recomendaciones (regularización, modelos más complejos, etc.)

---
