
## 1. Propósito del proyecto

En este entregable se desarrolla un dashboard en Power BI para analizar la información de ventas. El proceso parte de la carga de los archivos de origen, continúa con la limpieza y preparación de los datos y finaliza con la construcción del modelo de datos y las visualizaciones que facilitan la interpretación de los resultados.

El dashboard permite consultar información relacionada con las ventas por región y producto, así como revisar indicadores generales y promedios semanales.

## 2. Objetivo

Construir un dashboard interactivo en Power BI que permita visualizar y analizar los datos de ventas, utilizando información integrada de las tablas de categorías, calendario, ventas, productos y segmentos.

Para lograrlo, se busca:

- Cargar los archivos de información en Power BI.
- Limpiar y preparar los datos antes de construir el modelo.
- Identificar las variables y llaves relevantes de cada tabla.
- Establecer las relaciones entre las tablas mediante sus llaves.
- Construir el modelo de datos y su diagrama de relaciones.
- Crear indicadores, gráficas y tablas que permitan analizar los resultados.

## 3. Archivos de entrada

Para desarrollar el dashboard se utilizan los siguientes archivos:

```text
├── DIM_CATEGORY.csv
├── DIM_CALENDAR.xlsx
├── FACT_SALES.csv
├── DIM_PRODUCT.xlsx
└── DIM_SEGMENT.xlsx
```

Estos archivos contienen la información necesaria para integrar los datos de ventas con las dimensiones de categoría, calendario, producto y segmento.

## 4. Herramientas utilizadas

- **Power BI Desktop:** carga, transformación, modelado y visualización de los datos.
- **Modelo de datos de Power BI:** definición de relaciones entre las tablas y organización de las llaves.

## 5. Desarrollo del proyecto

### 5.1. Carga de los archivos

Se importan en Power BI los cinco archivos de origen: DIM_CATEGORY, DIM_CALENDAR, FACT_SALES, DIM_PRODUCT y DIM_SEGMENT.

Cada archivo se incorpora al proyecto para revisar su estructura, los campos disponibles y la calidad de sus registros.

### 5.2. Limpieza y preparación de los datos

Antes de construir el modelo, se realiza la limpieza de los datos Esta etapa es necesaria para evitar inconsistencias que puedan afectar las relaciones entre tablas o los resultados de las visualizaciones.

Se revisan los tipos de datos, los valores nulos, los registros duplicados y la consistencia de los campos que se utilizarán para relacionar las tablas. También se verifica que las columnas que funcionan como llaves tengan formatos compatibles.

Las transformaciones específicas deben corresponder a las condiciones encontradas en los archivos de origen.

### 5.3. Identificación de variables y llaves

Después de la limpieza, se identifican los campos que permiten conectar las tablas y los atributos que se utilizarán en el análisis.

Se revisan las llaves primarias de las tablas de dimensión y los campos relacionados en la tabla de hechos. Estas llaves permiten establecer las relaciones necesarias para integrar la información.

### 5.4. Construcción del modelo de datos

Con las tablas preparadas, se construye el modelo de datos en Power BI. En la vista de modelo se organizan las tablas y se establecen las relaciones correspondientes mediante los campos identificados.

El diagrama permite observar cómo se conecta la tabla de hechos FACT_SALES con las tablas de dimensiones. La correcta definición de estas relaciones permite utilizar campos de distintas tablas en los filtros, indicadores y gráficas del dashboard.

### 5.5. Diseño de las visualizaciones

Una vez construido el modelo, se selecciona la información de mayor interés para el usuario y se crean las visualizaciones correspondientes.

El dashboard presentado incluye:

- **Filtros de Año y Región:** permiten segmentar la información mostrada.
- **Indicador Total de ventas:** presenta el importe total de ventas.
- **Gráfica de Prom. Semanal Unidades por Código Producto:** muestra el comportamiento de las unidades promedio semanales por producto.
- **Indicador Promedio de ventas por semana:** presenta el promedio semanal mediante un medidor.
- **Tabla de resultados por producto:** muestra Código Producto, Unidades Vendidas, Ventas Totales ($) y Prom. Semanal Unidades.
- **Gráfica de Unidades Vendidas por Región:** permite comparar las unidades vendidas entre las regiones.

### 5.6. Análisis del dashboard

Las visualizaciones permiten consultar los resultados desde distintas perspectivas. Los filtros de Año y Región facilitan la segmentación; los indicadores ofrecen una vista general de las ventas y los promedios; y las gráficas y la tabla permiten profundizar en el comportamiento por producto y región.

De esta manera, el usuario puede explorar la información y comparar los resultados sin consultar directamente cada archivo de origen.

## 6. Resultado del proyecto

Como resultado se obtiene un dashboard en Power BI denominado **Análisis Regional y Producto**, acompañado de un modelo de datos que integra los cinco archivos de entrada.

El reporte contiene filtros, indicadores, una tabla de detalle por código de producto y gráficas para analizar las unidades vendidas por región y el promedio semanal de unidades por producto.

## 7. Conclusión

La creación del dashboard permite integrar la información de ventas y sus dimensiones en un solo modelo de análisis. Mediante la limpieza de los archivos, la identificación de llaves, la construcción del diagrama de relaciones y el diseño de visualizaciones, se facilita la consulta e interpretación de los resultados por producto y región.

## 8. Estructura general del proyecto

```text
Proyecto/
│
├── DIM_CATEGORY.csv
├── DIM_CALENDAR.xlsx
├── FACT_SALES.csv
├── DIM_PRODUCT.xlsx
├── DIM_SEGMENT.xlsx
│
└── Dashboard Power BI
    └── Análisis Regional y Producto
```
