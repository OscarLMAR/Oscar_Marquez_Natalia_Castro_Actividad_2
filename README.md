
# **Procesamiento de datos en una infraestructura cloud**

### **EVIDENCIA DE APRENDISAJE 1, 2 y 3**

**INTEGRANTES:**

**OSCAR LUIS MARQUEZ ARRIETA**

**NATALIA JADITH CASTRO OSPINO**

**PREICA2502B020061**

## **PROBLEMATICA**

La empresa de fluido electrico EnergyCol especializada en el servicio de energia electrica a gran parte de las regiones de colombia, tanto residenciales como comerciales. Esta presentando problemas con el procesamineto de los datos de todos los clientes debido al alto tamaño de informacion que se tienen de todos los clientes.

Debido al a esta problematica, se implementara una base de datos bien estructurada y organiza, que permita implementar toda la informacion que se requiera de los usuarios. Esto le brindara a la empresa una mejor organizacion y las relaciones entre el tamaño del edificio, la ocupación, la ubicación geográfica y los costos de energía.

## **Dataset**

**Fuente:** Kaggle: Residential and Commercial Energy Cost Dataset

**Enlace:** https://www.kaggle.com/datasets/andreylss/residential-and-commercial-energy-cost-dataset

# **VARIABLES RELEVANTES**

**id_cliente:** Identificador único para cada cliente

**tipo_cliente:** Tipo de propiedad (residencial o comercial)

**costo_energía_brl:** Costo mensual de energía en moneda local

**tipo_cliente:** Tipo de propiedad (residencial o comercial)

**regiones:** Región geográfica (Norte, Noreste, Medio Oeste, Sudeste, Sur)

🧰 **Tecnologías Utilizadas**

🚀 **Databricks Community Edition**

- Plataforma unificada para análisis y procesamiento de datos

- Entorno gestionado para ejecutar SQL, PySpark y Delta Lake

- Incluye:

- Databricks Runtime (según configuración del clúster)

- Notebooks colaborativos

- DBFS y Volumes como sistema de almacenamiento

🔥 **Apache Spark**

- Motor distribuido para procesamiento de datos a gran escala

- Utilizado mediante

- Spark SQL para consultas, DDL y validación

- DataFrames de PySpark para análisis y profiling

- Optimización mediante Catalyst Optimizer

💾 **Delta Lake**

- Formato de almacenamiento transaccional

- Beneficios aplicados

- Transacciones ACID

- Versionado de datos

- Lectura y escritura eficiente

- Compatibilidad completa con SQL en Databricks

🧮 **SQL (Spark SQL)**

- Utilizado para

- Creación de tablas con CREATE TABLE USING DELTA

- Inserción de datos mediante INSERT INTO

- Validación estructural con DESCRIBE TABLE y SHOW CREATE TABLE

- Consultas analíticas con GROUP BY y funciones agregadas

🐍 **PySpark**

- Utilizado para validaciones técnicas

- df.printSchema()

- df.describe().show()

- groupBy con agregaciones

- Lectura del archivo CSV con esquema inferido o definido

- Exploración del dataset mediante DataFrames

📂 **DBFS – Databricks File System**

- Sistema de almacenamiento utilizado en el proyecto

- Se usó para

- Guardar el archivo CSV subido manualmente

- Almacenar las tablas Delta generadas

- Ruta utilizada

- /Volumes/workspace/bigdata/semana3/energy_consumption.csv

📌 **Resumen General del Proyecto**

- Se implementó un pipeline completo de big data en Databricks

- Se cargó el dataset original en formato CSV hacia DBFS / Volumes

- Se diseñó y creó un modelo normalizado compuesto por tablas Delta

- Se llenaron las tablas mediante SQL usando una vista temporal del CSV

- Se realizaron validaciones en SQL y PySpark para asegurar calidad de datos

- Se documentó la infraestructura, carga, persistencia y consultas del proyecto
