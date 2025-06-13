# 🏗️ ETL Lakehouse con Delta Lake en Databricks

Este proyecto demuestra una arquitectura **Lakehouse** implementada sobre **Databricks** utilizando **Delta Lake**, simulando un flujo ETL completo para datos de ventas de retail.

---

## 🎯 Objetivo

Aplicar un pipeline moderno de ingeniería de datos usando la arquitectura **Medallion** (Bronze → Silver → Gold), aprovechando funcionalidades clave de Delta Lake como:

- **Merge incremental (UPSERT)**
- **Time Travel**
- **Transacciones ACID**
- **Formato optimizado Delta**

---

## 🧱 Estructura del Proyecto

| Notebook                        | Descripción |
|-------------------------------|-------------|
| `CSVtoParquet.ipynb`           | Conversión inicial de archivos CSV a Parquet para su posterior procesamiento. |
| `bronze_retail.ipynb`          | Ingesta de datos crudos (raw) en formato Delta Lake. |
| `retail_silver.ipynb`          | Limpieza, filtrado y enriquecimiento de datos para la capa Silver. |
| `Silver merge incremental.ipynb` | Simulación de una carga incremental usando `MERGE INTO` sobre Delta Lake. |
| `retail_gold.ipynb`            | Agregación de datos listos para análisis en la capa Gold. |
| `Time Travel Retail.ipynb`     | Ejemplo práctico de recuperación de versiones históricas con Delta Lake. |

---

## 🧰 Tecnologías y Herramientas

- Databricks Community Edition
- Apache Spark (PySpark)
- Delta Lake
- Arquitectura Medallion (Bronze / Silver / Gold)

---

## 🚀 Cómo usar este proyecto

1. Crear un entorno gratuito en [Databricks Community](https://community.cloud.databricks.com).
2. Subir los notebooks `.ipynb` al repositorio de tu Workspace.
3. Ejecutar los notebooks en orden según el flujo ETL.
4. Explorar las funcionalidades de Delta Lake (merge, versionado, optimización).

---

## 📌 Resultados clave

- Transformaciones eficientes con PySpark
- Actualizaciones incrementales simuladas
- Auditoría y versionado de datos usando Time Travel
- Organización de datos para análisis y consumo

---

## 📫 Contacto

Desarrollado por **John Castillo Reupo**  
[LinkedIn](https://www.linkedin.com/) • [GitHub](https://github.com/Johnkl725)

---

## 📌 Nota

Este proyecto fue desarrollado como práctica personal para fortalecer mis habilidades en **arquitectura de datos moderna**, **Big Data** y **Delta Lake** en la nube.
