![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python)
![Google Colab](https://img.shields.io/badge/Google%20Colab-SaaS%20Platform-orange?logo=googlecolab)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Active-success?logo=scikitlearn)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-purple?logo=pandas)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-blueviolet?logo=seaborn)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Modeling-yellow?logo=scikitlearn)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Graphs-lightblue?logo=plotly)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-red?logo=jupyter)
![GitHub](https://img.shields.io/badge/Repository-ml--analysis--colab-black?logo=github)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?logo=checkmarx)



# 🩺 Análisis y Predicción de Enfermedad Cardíaca con Machine Learning  
**Computación en la Nube — Actividad 5 (SaaS)**  
**Autor:** *Bairon Carrillo]*  
**Fecha:** *[31 de octubre de 2025]*  

---

## 🧠 Descripción del Proyecto
Este proyecto implementa un **análisis completo de datos médicos** mediante **Google Colab** como plataforma *Software as a Service (SaaS)*, aplicando algoritmos de **Machine Learning supervisado** para la **predicción de enfermedades cardíacas**.  

El objetivo principal fue explorar un conjunto de datos clínicos, identificar patrones relevantes y entrenar modelos predictivos que permitan estimar la probabilidad de que un paciente presente una enfermedad cardíaca, todo dentro del entorno en la nube proporcionado por Google Colab.

---

## 🎯 Objetivos
- Utilizar **Google Colab (SaaS)** como entorno de análisis y modelado.  
- Realizar **Exploración de Datos (EDA)** con estadísticas y visualizaciones.  
- Aplicar **modelos de Machine Learning supervisado**.  
- Comparar el rendimiento de distintos algoritmos.  
- Generar conclusiones basadas en evidencia y datos.  
- Documentar el proceso de forma reproducible.  

---

## 📊 Dataset Utilizado y Justificación
**Nombre:** *Heart Disease Dataset (Cleveland)*  
**Fuente:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Heart+Disease)  
**Tamaño:** 303 registros, 14 variables clínicas.  

**Justificación:**  
Se seleccionó este dataset por su relevancia médica y su estructura equilibrada para problemas de clasificación binaria. Permite demostrar el uso de modelos predictivos en el ámbito de la salud, un campo donde el *Machine Learning* tiene alto impacto social y académico.

---

## 💼 Problema de Negocio Abordado
La **predicción temprana de enfermedades cardíacas** puede reducir significativamente los riesgos de mortalidad y mejorar la toma de decisiones médicas.  
Este proyecto busca determinar **si un paciente tiene o no una enfermedad cardíaca** a partir de variables clínicas como edad, colesterol, presión arterial, frecuencia cardíaca, entre otras.

---

## ⚙️ Metodología Aplicada (Paso a Paso)
1. **Configuración inicial:** Importación de librerías, montaje de Google Drive, verificación de GPU.  
2. **Carga de datos:** Lectura del dataset desde UCI, renombrado de columnas y revisión de estructura.  
3. **Exploración de Datos (EDA):** Estadísticas descriptivas, detección de valores faltantes y *outliers*, generación de 5+ visualizaciones (histogramas, boxplots, correlación, dispersión).  
4. **Preprocesamiento:** Imputación de valores faltantes, codificación de variables categóricas, escalado con `StandardScaler`, y división *train/test*.  
5. **Modelado:** Entrenamiento y evaluación de **Regresión Logística** y **Random Forest Classifier**.  
6. **Optimización:** Ajuste de hiperparámetros mediante `GridSearchCV`.  
7. **Evaluación:** Cálculo de métricas (Accuracy, Precision, Recall, F1, ROC-AUC), matrices de confusión y curvas ROC.  
8. **Conclusiones:** Interpretación de resultados, recomendaciones y reflexión sobre el uso de SaaS.  

---

## 🤖 Algoritmos de Machine Learning Utilizados y Justificación
| Algoritmo | Tipo | Justificación |
|------------|------|----------------|
| **Regresión Logística** | Clasificación lineal | Proporciona interpretabilidad y una línea base robusta. |
| **Random Forest** | Ensamble de árboles | Ofrece mayor precisión, maneja relaciones no lineales y reduce el sobreajuste. |

---

## 🔍 Principales Hallazgos y Patrones Identificados
- Mayor riesgo de enfermedad en personas **mayores de 50 años**.  
- **Colesterol alto** y **baja frecuencia cardíaca máxima (thalach)** se asocian a mayor probabilidad de enfermedad.  
- Las variables `cp` (tipo de dolor en el pecho) y `exang` (angina inducida por ejercicio) resultaron altamente predictivas.  
- **Random Forest** superó a la Regresión Logística con mejor *recall* y *AUC*, demostrando mayor capacidad de detección.  

---


---

## ⚡ Instrucciones para Reproducir el Análisis
1. Abre el notebook en [Google Colab](https://colab.research.google.com).  
2. Conecta el entorno a GPU (opcional).  
3. Ejecuta todas las celdas en orden (`Runtime > Run all`).  
4. Si es necesario, monta tu Google Drive y actualiza la ruta de los datos.  
5. Revisa los resultados en las secciones de EDA, Modelado y Conclusiones.

**Dependencias principales:**
```bash
pip install pandas numpy seaborn matplotlib scikit-learn plotly

