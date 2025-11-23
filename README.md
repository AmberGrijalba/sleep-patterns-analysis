# sleep-patterns-analysis
# 💤 Análisis de Hábitos de Sueño y Estilo de Vida
#📌 Descripción del Proyecto

Este proyecto realiza un análisis exploratorio de datos (EDA) sobre un conjunto de información relacionado con hábitos de sueño, estilo de vida y niveles de estrés.
El objetivo es identificar patrones y relaciones entre variables que puedan explicar cómo factores como la duración del sueño, calidad del descanso y actividad física se asocian con el estrés.

Este análisis servirá como base para un futuro modelo de clasificación que prediga el nivel de estrés de una persona según sus hábitos.

#🎯 Objetivos Principales

✅ Comprender la estructura del dataset y su contenido
✅ Analizar distribuciones de variables numéricas y categóricas
✅ Detectar outliers y limpiar los datos
✅ Crear una variable objetivo binaria asociada al estrés
✅ Evaluar relaciones entre variables (análisis bivariante y correlación)
✅ Dividir los datos en entrenamiento y prueba para modelado
✅ Guardar datasets procesados para uso posterior

#🗂️ Dataset Utilizado

Fuente: Kaggle
https://www.kaggle.com/datasets/minahilfatima12328/lifestyle-and-sleep-patterns

### Contenido del dataset:
Incluye variables como:

Edad

Género

Duración del sueño

Calidad del sueño

Actividad física

Nivel de estrés

Ritmo cardíaco

Presión arterial

Pasos diarios

Trastornos del sueño

Entre otras

Filas y columnas: Variable según versión descargada.

# 🔧 Pasos del Análisis Realizado
## ✅ 1. Carga y Exploración Inicial

Lectura del dataset

Identificación de tipos de variables

Revisión de valores nulos

Descripción estadística inicial

Objetivo: entender la estructura del dataset antes de transformarlo.

## ✅ 2. Limpieza y Transformaciones

Separación de presión arterial en sistólica/diastólica

Tratamiento de valores faltantes (si aplica)

Eliminación de valores extremos usando IQR

Objetivo: evitar distorsiones y mejorar la calidad del análisis.

## ✅ 3. Análisis Univariante

Gráficas de distribución para variables numéricas

Gráficas de barras para variables categóricas

Conclusión clave: se observaron patrones de sueño y actividad con variaciones importantes entre individuos.

## ✅ 4. Creación de la Variable Objetivo (Estrés)

Se transformó la variable numérica de estrés en una clasificación binaria:

Valor original	Nueva categoría
3 – 6	ESTRES MODERADO
≥ 7	ESTRESADO

Luego se eliminó la variable numérica original.

Objetivo: preparar el dataset para un futuro modelo de clasificación.

## ✅ 5. Análisis Bivariante

Comparación del estrés binario contra todas las variables

Boxplots, barras y proporciones

Hallazgos clave:

Menos horas de sueño → mayor proporción de estresados

Peor calidad del sueño → mayor estrés

Menor actividad física → mayor estrés

## ✅ 6. Matriz de Correlación

Identificación de variables redundantes

Eliminación de variables con alta correlación y poco aporte

Objetivo: simplificar el dataset y evitar colinealidad.

## ✅ 7. División Train/Test

80% entrenamiento

20% prueba

Estratificación según nivel de estrés

Resultado: proporciones equilibradas entre ambas clases.

## ✅ 8. Exportación Final

### Se guardaron dos archivos procesados:

data/train_sleep_stress.csv
data/test_sleep_stress.csv


Estos serán utilizados en la etapa de modelado.

# 📊 Resultados Generales

El estrés está presente en la mayoría de los individuos

Dormir menos y tener peor calidad de sueño se asocia a mayor estrés

La actividad física podría actuar como factor protector

El dataset quedó limpio, balanceado y listo para Machine Learning

🚀 Próximos Pasos

✅ Construir un modelo de clasificación
✅ Evaluar métricas de desempeño
✅ Implementar interpretabilidad del modelo
✅ Publicar resultados en la web

👤 Autor

Amber Grijalba (Ambervg4733@gmail.com)
Proyecto académico de análisis de datos
