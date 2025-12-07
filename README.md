# Profession Mention Detection in Spanish Tweets  
**A Natural Language Processing project using Transformer-based models**

Este proyecto desarrolla un sistema de clasificación automática para identificar si un tweet en español contiene una **mención explícita a una profesión**.  
El objetivo es demostrar cómo los modelos de lenguaje modernos pueden aplicarse a análisis semánticos específicos dentro de textos breves e informales, como los que se encuentran en redes sociales.

---

## Objetivo del proyecto

Diseñar y entrenar un **clasificador binario** capaz de:

- Recibir un tweet como entrada  
- Analizar su contenido textual  
- Determinar si menciona al menos una profesión (1) o no (0)  

El pipeline completo incluye análisis exploratorio, preprocesamiento, selección de modelo, fine-tuning y generación de predicciones.

---

## Tecnologías y librerías utilizadas

- **Python 3.10+**  
- **Hugging Face Transformers** (fine-tuning de modelos preentrenados)  
- **Datasets** (gestión eficiente del dataset)  
- **Scikit-learn** (métricas y evaluación)  
- **Pandas / NumPy** (procesamiento de datos)  
- **Matplotlib / Seaborn / WordCloud** (visualización)  
- **Google Colab** o Jupyter Notebook  

---

## Metodología

### 1️⃣ Exploración del dataset  
- Análisis estadístico inicial  
- Distribución de clases  
- Longitud y variabilidad de los textos  
- Visualización de patrones léxicos  

### 2️⃣ Preprocesamiento del texto  
- Tokenización con el modelo seleccionado  
- Limpieza mínima para preservar la semántica original  
- Preparación de splits para entrenamiento/validación/test  

### 3️⃣ Entrenamiento del modelo  
- Selección de un *transformer* optimizado para español  
- Configuración de hiperparámetros (epochs, batch size, learning rate)  
- Entrenamiento reproducible con `Trainer` de Hugging Face  

### 4️⃣ Evaluación  
- Cálculo de métricas estándar:  
  - Accuracy  
  - Precision  
  - Recall  
  - F1-score  
- Análisis del desempeño del modelo  

### 5️⃣ Generación de predicciones  
- Etiquetado del conjunto de prueba  
- Exportación del archivo `predictions.tsv` con las clases generadas  

---

## 📁 Estructura del repositorio

