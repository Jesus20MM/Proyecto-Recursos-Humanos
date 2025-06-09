# Predicción de Rotación de Personal con Modelos de Clasificación

## Descripción
Este proyecto aborda el problema de por qué los empleados abandonan la empresa. El objetivo es predecir la probabilidad de que un empleado renuncie, utilizando Python como herramienta principal.

Para resolver el problema, se aplicaron tres modelos de machine learning: regresión logística, bosques aleatorios y una red neuronal artificial. Se dio especial énfasis a la regresión logística, seleccionando el mejor umbral a analizando de la curva ROC mediante el análisis de la tasa de verdaderos positivos y falsos positivos para cada umbral. También se realizó un análisis detallado de la matriz de confusión. Además, se generaron visualizaciones complementarias para extraer información adicional de los datos.

## Dataset
El dataset tiene un conjunto de 35 variables, donde 34 de ellas son independientes y una dependiente. La dimensión del dataset es
(1470, 35). Todas las características son información de los clientes y nuestra variable objetivo es attrition (se marcha o no
se marcha)

## Metodología (meter imágenes si es necesario)
Describe los pasos principales del análisis o modelo, por ejemplo:
1. Análisis exploratorio de datos (EDA)
2. Limpieza y transformación de datos
3. Selección de características
4. Modelado (regresión, clasificación, clustering, etc.)
5. Evaluación del modelo

## Resultados
Modelo útil para decisiones médicas preventivas. Buen recall. Umbral optimizado.

## Lecciones aprendidas
- Manejo de desbalance de clases
- Importancia de elegir la métrica correcta
- Curva ROC y ajuste de umbral

## Tecnologías
Scikit-learn, Pandas, Numpy, Matplotlib, Seaborn

## Mejoras futuras
- Implementar descenso de gradiente
- Organizar el flujo con pipelines
