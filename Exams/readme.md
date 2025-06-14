# Exámenes de Ciencia de Datos

Este repositorio contiene tres exámenes de Ciencia de Datos. A continuación se detallan los datasets asignados a cada examen:

## Examen 1

- **Dataset Asignado**: `cliente.csv`
  - **Descripción**: Este dataset contiene información sobre clientes.
  - **Instrucciones**: Realizar el análisis y las tareas indicadas basándose en el dataset de clientes.

## Examen 2

- **Datasets Asignados**: `train_bigmart.csv`, `test_bigmart.csv`
  - **Descripción**: Este examen consta de dos datasets, uno de entrenamiento (`train`) y otro de prueba (`test`).
  - **Instrucciones**: Utilizar el dataset de entrenamiento para entrenar el modelo y luego probarlo utilizando el dataset de prueba.

## Examen 3

- **Datasets Asignados**: `intermoda.parquet`, `intermoda1.parquet`
  - **Descripción**: En el dataset adjunto se encuentra la información de ventas de dos periodos de venta X, los cuales usted como científico de datos tendrá que explorar, clasificar, limpiar y mostrar análisis o descubrimientos, tomando en cuenta los atributos que el set de datos le ofrece. Es importante que puede hacer presunciones de datos que no existen de ser necesario para su análisis.
  - **Instrucciones**: En el presente documento se presentará una prueba técnica necesaria para el proceso de selección al puesto científico de datos. Deberá realizarla en el tiempo establecido y enviar la solución por correo electrónico con las evidencias solicitadas a continuación.
 

## Examen 4

- **Datasets Asignados**: `bank-additional-full.csv`
  - **Descripción**: Evaluar los datos realizando un análisis descriptivo y evaluar una serie de modelos de clasificación. El objetivo final es elegir el modelo que mejor resultados obtiene prediciendo la columna 21, que representa si el cliente se suscribe al servicio correspondiente. El objetivo de clasificación binaria es predecir si el cliente suscribirá un depósito a plazo (variable y)


## Examen 5

- **Datasets Asignados**: `visitas_sucursal.csv`, `zonas.csv`
  - **Descripción**: El banco PY está enfrentando un problema de retención de clientes. A partir de un experimento, se identificó que una vez que el cliente expresa su intención de darse de baja, ya no es posible revertir la situación. Se busca anticiparse a este comportamiento desarrollando un modelo que permita identificar, antes de que ocurra, si un cliente tiene alta probabilidad de darse de baja.
  - **Instrucciones**: 
    - Desarrollar un modelo de Machine Learning que prediga el churn del cliente.
    - Justificar la elección del algoritmo utilizado.
    - Evaluar el rendimiento del modelo y justificar si es apto para salir a producción.
    - Analizar las variables que más influyen en la predicción.
    - Definir cómo y cuándo se utilizaría el modelo en el flujo operativo.
    - Determinar si existe overfitting o underfitting.
    - Tener en cuenta los siguientes valores económicos en las decisiones:
      - `costo_retencion = 20`
      - `rentabilidad_corto = 8` (primeros 3 meses)
      - `rentabilidad_largo = 50` (primer año)
      - `rentabilidad_baja = -2` (cuando el cliente se da de baja)
