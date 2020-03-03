# Sistemas Inteligentes para la Gestión en la Empresa
# MaterialP1SIGE2020


Dataset: [25Mb](./dataset/LoanStats_2017Q4.csv.zip) 120K rows, 148 features, classification.

Transactions ID and identity ID: https://www.kaggle.com/c/ieee-fraud-detection/data


# Práctica 1: Pre-procesamiento de datos y clasificación binaria

## Curso 2019-2020

# Objetivos y evaluación

En esta primera práctica de la asignatura Sistemas Inteligentes para la Gestión en la Empresa estudiaremos cómo realizar diversas tareas de pre-procesamiento de datos, como paso previo e imprescindible para el aprendizaje automático.

La práctica consistirá en la resolución de un problema de pre-procesamiento y aprendizaje automático. **Junto a la solución del problema (código R), se entregará una memoria explicativa de las tareas realizadas.**

La práctica se desarrollará de forma individual. La calificación constituirá el 15% de la nota final de la asignatura (1.5 puntos). Se evaluará, en este orden: (1) la aproximación al problema y la evaluación de alternativas; (2) la calidad de la memoria presentada; (3) la precisión y la exactitud obtenida por el clasificador. Se valorará especialmente la claridad en la redacción y en la presentación del trabajo realizado.

La entrega se realizará a través de la plataforma docente de PRADO, en el enlace que se habilitará al efecto.

# Descripción del problema

Se trabajará sobre el conjunto de datos de préstamos proporcionado junto a este guion, que es una variación del ofrecido en la competición de Kaggle IEEE-CIS Fraud Detection ([https://www.kaggle.com/c/ieee-fraud-detection/data](https://www.kaggle.com/c/ieee-fraud-detection/data)).

La descripción de las variables de este conjunto de datos se encuentra en la sección _Data_ de esta misma web.

El problema consiste en predecir si una transacción online es fraudulenta o no (_isFraud_) a partir del resto de variables. Los datos están separados en dos ficheros:

	- _transaction_, con los datos de la propia transacción (393 variables + 1 identificador de transacción)

	- _identity_, con los datos de identidad de la persona que realiza la transacción (40 variables + 1 identificador de transacción asociada)

Ambos ficheros pueden combinarse a través del atributo _TransactionID_. No todas las transacciones tienen asociada información de identidad. A su vez, los ficheros aparecen ya separados en conjuntos de entrenamiento y validación.

El ejercicio se abordará como un problema de clasificación binaria, con dos posibles salidas: {_Yes_, _No_}. La selección de datos y el procesamiento queda a criterio del estudiante.

La memoria explicará qué **tareas de pre-procesamiento** se han llevado a cabo y con qué objetivo, así como los resultados obtenidos. Se enumeran a continuación de forma no exhaustiva algunas de las tareas que pueden realizarse:

- Transformación y limpieza de valores numéricos
- Selección de variables
	- Variables con valores perdidos
	- Variables con ‘mucha’ diversidad en sus valores
	- Variables con ‘poca’ diversidad en sus valores
	- Variables correladas
	- Variables importantes según técnicas avanzadas
- Detección de conflictos e inconsistencias en los datos
	- Identificación y tratamiento de ‘outliers’
	- Identificación e imputación de valores perdidos
	- Tratamiento del ruido
	- Normalización y discretización
- Reducción y ampliación de datos
	- Selección de características
	- Selección de ejemplos
	- Tratamiento de clases no balanceadas
- Visualización de datos

La memoria explicará qué **técnicas de clasificación se han utilizado**. Al menos se **utilizarán dos técnicas diferentes**, cuya selección deberá justificarse. También se detallará el proceso de generación de los conjuntos de entrenamiento, validación y test. Se analizarán los resultados obtenidos con las técnicas utilizadas, haciendo especial énfasis en las medidas de precisión y exhaustividad. También se discutirá el impacto del pre-procesamiento en los resultados de clasificación.

Se recomienda apoyar las explicaciones con *gráficos, diagramas, etc.*

# Entrega

**Límite**: 3 de abril de 2020

**Contenidos**: Un fichero .zip, incluyendo:

**Código en R (.R, .Rmd)**

- Memoria
	- Portada: nombre, título
	- Índice
	- Contenidos (no exhaustivamente)
		- Exploración
		- Pre-procesamiento
		- Clasificación
		- Discusión de resultados
		- Conclusiones
		- Bibliografía
