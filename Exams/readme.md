# Exámenes de Ciencia de Datos

Este repositorio contiene seis exámenes de Ciencia de Datos. A continuación se detallan los datasets asignados a cada examen:

---

## Examen 1

- **Dataset Asignado**: `cliente.csv`  
  - **Descripción**: Este dataset contiene información sobre clientes.  
  - **Instrucciones**: Realizar el análisis y las tareas indicadas basándose en el dataset de clientes.

---

## Examen 2

- **Datasets Asignados**: `train_bigmart.csv`, `test_bigmart.csv`  
  - **Descripción**: Este examen consta de dos datasets, uno de entrenamiento (`train`) y otro de prueba (`test`).  
  - **Instrucciones**: Utilizar el dataset de entrenamiento para entrenar el modelo y luego probarlo utilizando el dataset de prueba.

---

## Examen 3

- **Datasets Asignados**: `intermoda.parquet`, `intermoda1.parquet`  
  - **Descripción**: En el dataset adjunto se encuentra la información de ventas de dos periodos de venta X, los cuales usted como científico de datos tendrá que explorar, clasificar, limpiar y mostrar análisis o descubrimientos, tomando en cuenta los atributos que el set de datos le ofrece. Es importante que puede hacer presunciones de datos que no existen de ser necesario para su análisis.  
  - **Instrucciones**: En el presente documento se presentará una prueba técnica necesaria para el proceso de selección al puesto científico de datos. Deberá realizarla en el tiempo establecido y enviar la solución por correo electrónico con las evidencias solicitadas a continuación.

---

## Examen 4

- **Dataset Asignado**: `bank-additional-full.csv`  
  - **Descripción**: Evaluar los datos realizando un análisis descriptivo y evaluar una serie de modelos de clasificación. El objetivo final es elegir el modelo que mejor resultados obtiene prediciendo la columna 21, que representa si el cliente se suscribe al servicio correspondiente. El objetivo de clasificación binaria es predecir si el cliente suscribirá un depósito a plazo (variable `y`).

---

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

---

## Examen 6

- **Dataset Asignado**: `hotels.csv`  
- **Fuente**: [Antonio, Almeida y Nunes (2019)](https://www.sciencedirect.com/science/article/pii/S2352340918315191?via%3Dihub)  

**Descripción:**  
Este examen se basa en datos reales de reservas de hotel entre julio de 2015 y agosto de 2017. Se proporciona un dataset unificado de dos hoteles distintos:  
- **H1:** Hotel tipo resort  
- **H2:** Hotel urbano  

Ambos conjuntos tienen la misma estructura, con 23 variables y un total combinado de casi 50.000 observaciones. Cada fila representa una reserva, incluyendo tanto estancias efectivas como cancelaciones. Se han eliminado todos los elementos de datos que pudieran identificar al hotel o al cliente.

---

### Objetivos del Examen

#### Parte 1 – Análisis Exploratorio de Datos (EDA)

Durante esta parte, debes realizar un análisis exploratorio exhaustivo del dataset con foco en:

- **Control de calidad de datos:** Verifica valores nulos, tipos incorrectos, outliers, datos inconsistentes, etc.  
- **Propuesta de acciones correctivas:** En caso de detectar problemas en los datos, documenta cómo planeas corregirlos o imputarlos.  
- **Descubrimiento de patrones:** Describe insights relevantes desde la perspectiva del negocio hotelero.  
- **Visualización de datos:** Se requiere generar **al menos 10 gráficos** usando cualquier biblioteca (`matplotlib`, `seaborn`, `plotly`, etc.), y **explicar cada uno claramente**.

---

#### Parte 2 – Ingeniería de Features y Modelado

El objetivo aquí es construir un modelo que prediga si una reserva incluyó **niños y/o bebés**.

**Requisitos:**

- Crear **tres transformadores personalizados** en un archivo `transformers.py`. Estos deben:  
  - Generar nuevas features útiles (ejemplo: `total_nights` = `stays_in_week_nights` + `stays_in_weekend_nights`)  
  - Corregir errores o inconsistencias en los datos (ejemplo: transformar `'0'` string a `0` int)  
- Implementar un pipeline completo en un archivo `pipelines.py` que:  
  - Integre los transformadores anteriores  
  - Prepare los datos para el entrenamiento  
  - Entrene el modelo  
- Entrenar al menos **tres modelos de Machine Learning** distintos  
- Usar la variable objetivo derivada: `children + babies > 0` (clasificación binaria)  
- Evaluar modelos usando métricas relevantes: accuracy, precision, recall, F1-score, etc.

---

#### Parte 3 – Presentación de Resultados

El objetivo es comunicar los hallazgos a stakeholders no técnicos.

**Se espera:**

- **Resumen del EDA:** ¿Qué descubriste en la exploración de datos?  
- **Explicación de features:** ¿Qué nuevas variables se crearon y por qué?  
- **Resumen del rendimiento de modelos:** ¿Cuál funcionó mejor? ¿Por qué?  
- **Formato libre:** Puedes presentar estos resultados al final del notebook o en otro formato como:  
  - PDF  
  - Presentación (PPT)  
  - Documento externo (Google Docs, Notion, etc.)

---

### Requisitos Técnicos

- Python 3.x  
- Pandas 1.x o superior  
- Scikit-learn  
- Bibliotecas de visualización (`matplotlib`, `seaborn`, `plotly`, etc.)  
- Uso de entorno virtual (`venv` o `conda`)  
- Entrega en carpeta ZIP o repositorio público/privado (GitHub, GitLab, etc.) incluyendo:  
  - Notebook principal (`.ipynb`)  
  - Scripts (`pipelines.py`, `transformers.py`)  
  - Archivos auxiliares (PDF, imágenes, slides, etc.)  
  - Archivo `requirements.txt` o `environment.yml`

---

### Aspectos Deseables (Nice to Have)

- Uso de Git para control de versiones  
- Explicabilidad del modelo con SHAP o herramientas similares  
- Buenas prácticas de programación en Python: funciones limpias, POO, documentación clara  
- Narrativa convincente que conecte el análisis con decisiones de negocio

---

## ¡Lo más importante!

**Diviértete resolviendo el desafío y demuestra tu capacidad analítica y técnica.**

