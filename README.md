# Telecom X - Análisis de evasión de clientes (Churn)

## Descripción del proyecto

Este proyecto tiene como objetivo analizar los factores asociados con la evasión de clientes (Churn) en una empresa de telecomunicaciones ficticia llamada Telecom X.

La evasión de clientes representa uno de los principales desafíos para empresas que operan bajo modelos de suscripción, ya que la pérdida constante de clientes puede afectar directamente los ingresos y la estabilidad del negocio.

A través de técnicas de análisis de datos utilizando Python y Pandas, se realiza un proceso completo de exploración, limpieza y análisis de la información disponible con el objetivo de identificar patrones que puedan explicar el comportamiento de los clientes.

---

## Objetivos del análisis

- Analizar el comportamiento de los clientes de Telecom X.
- Identificar variables asociadas con la evasión de clientes.
- Explorar patrones relacionados con contratos, servicios y facturación.
- Generar insights que puedan ayudar a reducir la tasa de cancelación.

---

## Tecnologías utilizadas

Este proyecto fue desarrollado utilizando las siguientes herramientas:

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Jupyter Notebook  
- Google Colab  

---

## Dataset

Los datos utilizados en este proyecto provienen de un dataset en formato JSON que contiene información sobre los clientes de Telecom X.

El dataset incluye variables como:

- Información demográfica del cliente
- Servicios contratados
- Tipo de contrato
- Método de pago
- Facturación mensual
- Facturación total
- Estado de churn (cancelación del servicio)

Fuente de los datos:

https://github.com/alura-cursos/challenge2-data-science-LATAM

---

## Proceso de análisis

El análisis del dataset se realizó siguiendo varias etapas comunes dentro de un flujo de trabajo de análisis de datos.

### 1. Extracción de datos

Los datos fueron cargados desde un archivo JSON utilizando la biblioteca Pandas en Python.

Posteriormente se transformó la estructura del JSON en un formato tabular para facilitar su manipulación y análisis.

---

### 2. Exploración inicial del dataset

Durante esta etapa se analizaron las características generales del dataset utilizando funciones como:

- `DataFrame.info()`
- `DataFrame.describe()`
- `DataFrame.dtypes`

Esto permitió comprender la estructura de los datos, los tipos de variables disponibles y detectar posibles inconsistencias.

---

### 3. Limpieza y preparación de datos

En esta etapa se realizaron varias tareas de limpieza para asegurar la calidad de los datos:

- Identificación de valores nulos
- Verificación de registros duplicados
- Limpieza de nombres de columnas
- Conversión de tipos de datos
- Revisión de inconsistencias en variables categóricas

Estas transformaciones permitieron preparar el dataset para su análisis posterior.

---

### 4. Ingeniería de variables

Se creó una nueva variable llamada **Cuentas_Diarias**, calculada a partir de la facturación mensual de los clientes.

Esta variable permite analizar el gasto promedio diario de los clientes y obtener una perspectiva adicional sobre su comportamiento de consumo.

---

### 5. Análisis exploratorio de datos

Se realizaron diversas visualizaciones y análisis descriptivos para identificar patrones relacionados con la evasión de clientes.

Entre los análisis realizados se incluyen:

- Distribución del churn
- Churn según tipo de contrato
- Churn según método de pago
- Churn según servicios contratados
- Relación entre churn y facturación mensual
- Relación entre churn y gasto diario
- Análisis del tiempo de permanencia del cliente

Estas visualizaciones ayudaron a identificar tendencias importantes dentro del dataset.

---

## Principales insights

A partir del análisis exploratorio se identificaron algunos patrones relevantes:

- Los clientes con contratos de corto plazo presentan mayores tasas de cancelación.
- Los clientes con menor tiempo de permanencia muestran mayor probabilidad de churn.
- Algunas combinaciones de servicios presentan diferencias en la distribución del churn.
- El gasto mensual y el gasto diario muestran variaciones entre clientes que cancelan el servicio y los que permanecen.

Estos patrones permiten comprender mejor el comportamiento de los clientes y pueden servir como base para futuras estrategias de retención.

---

## Recomendaciones

Con base en los resultados obtenidos durante el análisis, se pueden considerar algunas acciones para reducir la evasión de clientes:

- Desarrollar modelos predictivos de churn para identificar clientes en riesgo.
- Implementar estrategias de retención enfocadas en clientes con menor tiempo de permanencia.
- Analizar la relación entre precios y cancelación del servicio.
- Evaluar combinaciones de servicios que favorezcan la permanencia del cliente.
- Segmentar clientes según su nivel de riesgo de cancelación.

---

## Trabajo futuro

Este análisis exploratorio representa un primer paso para comprender los factores asociados con la evasión de clientes.

Como continuación del proyecto, se podrían desarrollar nuevas líneas de trabajo como:

- Construcción de modelos predictivos de churn.
- Segmentación de clientes mediante técnicas de clustering.
- Análisis de correlación entre variables.
- Desarrollo de dashboards interactivos para monitorear indicadores clave.

---

## Estructura del proyecto

Telecom_X

data  
└── TelecomX_Data.json  

notebooks  
└── telecomx_churn_analysis.ipynb  

images  

README.md  

requirements.txt

---

## Cómo ejecutar el proyecto

Para ejecutar este proyecto en tu entorno local, sigue los siguientes pasos.

### 1. Clonar el repositorio

git clone https://github.com/tu_usuario/Telecom_X.git

### 2. Acceder al directorio del proyecto

cd Telecom_X

### 3. Instalar las dependencias

pip install -r requirements.txt

### 4. Abrir el notebook

Abrir el archivo ubicado en:

notebooks/telecomx_churn_analysis.ipynb

El análisis fue desarrollado en un entorno de Jupyter Notebook / Google Colab.

---

## Autor

Proyecto desarrollado por **Emilio Romero** como parte de un ejercicio de análisis de datos enfocado en el estudio de evasión de clientes utilizando Python y herramientas de ciencia de datos.
