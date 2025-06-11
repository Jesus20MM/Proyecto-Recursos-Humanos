## Descripción
Este proyecto aborda el problema de por qué los empleados abandonan la empresa. El objetivo es predecir la probabilidad de que un empleado renuncie, utilizando Python como herramienta principal.
Para resolver el problema, se aplicaron tres modelos de machine learning: regresión logística, bosques aleatorios y una red neuronal artificial. Se dio especial énfasis a la regresión logística, seleccionando el mejor umbral a analizando de la curva ROC mediante el análisis de la tasa de verdaderos positivos y falsos positivos para cada umbral. También se realizó un análisis detallado de la matriz de confusión. Además, se generaron visualizaciones complementarias para extraer información adicional de los datos.

## Dataset
El dataset tiene un conjunto de 35 variables, donde 34 de ellas son independientes y una dependiente. La dimensión del dataset es (1470, 35). Todas las características son información de los empleados como edad, departamento, educación, etc. y nuestra variable objetivo es attrition (se marcha o no se marcha).

## Metodología 
Describe los pasos principales del análisis o modelo, por ejemplo:
1.	Análisis exploratorio de datos (EDA)
En esta etapa conocimos en profundidad el dataset y planteamos preguntas clave orientadas al análisis, una vez definido el objetivo general del proyecto. La importancia de explorar exhaustivamente el dataset radica en comprender qué tipo de transformaciones o procesos de limpieza son necesarios para alcanzar nuestros fines. En este caso, el objetivo principal era obtener un conjunto de datos limpio y procesado para la implementación de modelos de clasificación, ya que buscábamos entender la deserción de empleados en términos de probabilidad. Esta fase nos permitió identificar patrones, valores atípicos y relaciones relevantes entre variables. El propósito del EDA es dejar completamente claros los pasos necesarios para transformar el dataset original en uno preparado para el análisis predictivo.
2.	Limpieza y transformación de datos
Dado que el dataset contenía información valiosa sobre los empleados, realizamos una limpieza exhaustiva con fines tanto exploratorios como de preparación para el modelado. Esto incluyó el tratamiento de valores nulos, codificación de variables categóricas, normalización y detección de outliers. Esta depuración nos permitió visualizar mejor el comportamiento de los empleados según sus características. Se generaron representaciones gráficas como histogramas, gráficos de densidad, mapas de calor para correlaciones y análisis de tendencias, lo cual enriqueció la comprensión general del conjunto de datos y facilitó una toma de decisiones más informada en las siguientes fases.
3.	Modelado (regresión, clasificación, clustering, etc.)
Con los datos ya procesados, realizamos pequeños ajustes adicionales antes de alimentar los modelos de clasificación. Se probaron enfoques tanto de aprendizaje automático como de aprendizaje profundo. Nos enfocamos en identificar adecuadamente las variables independientes y dependientes de acuerdo con el objetivo principal: predecir la probabilidad de deserción. Implementamos modelos de regresión logística, árboles de decisión y redes neuronales profundas para comparar su desempeño. Esta etapa fue clave para traducir los hallazgos del EDA en modelos predictivos útiles y accionables.
4.	Evaluación del modelo
Antes de evaluar los modelos, definimos los principales KPI’s (Key Performance Indicators) según las necesidades del problema. Utilizamos la matriz de confusión para analizar métricas como precisión, recall, F1-score, y ajustamos el umbral de decisión mediante la curva ROC (Receiver Operating Characteristic) y el área bajo la curva (AUC). Comparando el rendimiento entre modelos sin procesar y modelos optimizados, concluimos que la regresión logística sobre los datos procesados fue el modelo óptimo, a pesar de haber explorado alternativas más complejas como una red neuronal profunda. Esta elección se basó en un equilibrio entre rendimiento, interpretabilidad y facilidad de implementación.

## Resultados
Los resultados que se obtuvieron fue pasar de un modelo poco útil a un modelo posiblemente útil ya que se optimizó la sensibilidad y pudimos extremar la tasa de verdaderos positivos o Rcall.

Aquí se muestran los diferentes umbrales para la regresión logística:

![image](https://github.com/user-attachments/assets/9ac5bd42-23b9-4225-887b-4bd77a7fabf2)



## Lecciones aprendidas
- Manejo de desbalance de clases
- Importancia de elegir la métrica correcta
- Curva ROC y ajuste de umbral
- Métricas de la matriz de confusión 
- Implementación básica de un bosque aleatorio y red neuronal produnda

## Tecnologías
Pandas, Scikit-Learn, redes neuronales y tensorflow, visualizaciones, Numpy, matplotlib, seaborn, clasificación.
## Mejoras futuras
Comparar los resultados de los modelos en conjunto, métodos de evaluacion más robusto como validación cruzada, profundizar en la optimizacion de los modelos con sus parámetros e hiperparámetros, implementar el descenso del gradiente con la funcion de costes simplificada para la regresión, implementar XGBoost
