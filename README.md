# sql-data-warehouse-project
Construcción de un Data Warehouse moderno con SQL Server
# Proyecto de Almacenamiento y Análisis de Datos

¡Bienvenido al repositorio del **Proyecto de Almacenamiento y Análisis de Datos**! 🚀
Este proyecto demuestra una solución integral de almacenamiento y análisis de datos, desde la creación de un almacén de datos hasta la generación de información útil. Diseñado como un proyecto de portafolio, destaca las mejores prácticas de la industria en ingeniería y análisis de datos.

--- ## 🏗️ Arquitectura de Datos

La arquitectura de datos para este proyecto sigue las capas **Bronce**, **Plata** y **Oro** de la Arquitectura Medallion:
![Arquitectura de Datos](docs/data_architecture.png)

1. Capa **Bronce**: Almacena los datos sin procesar tal cual provienen de los sistemas de origen. Los datos se ingieren desde archivos CSV a una base de datos SQL Server.
2. Capa **Plata**: Esta capa incluye procesos de limpieza, estandarización y normalización de datos para prepararlos para el análisis.
3. Capa **Oro**: Contiene datos listos para el negocio, modelados en un esquema de estrella, necesarios para la elaboración de informes y análisis.

---

## 📖 Resumen del proyecto

Este proyecto incluye:

1. **Arquitectura de datos**: Diseño de un almacén de datos moderno utilizando las capas **Bronce**, **Plata** y **Oro** de la arquitectura Medallion.
2. **Pipelines ETL**: Extracción, transformación y carga de datos desde los sistemas de origen al almacén.
3. **Modelado de datos**: Desarrollo de tablas de hechos y dimensiones optimizadas para consultas analíticas.
4. **Análisis e informes**: Creación de informes y paneles basados ​​en SQL para obtener información útil.

🎯 Este repositorio es un excelente recurso para profesionales y estudiantes que buscan demostrar su experiencia en:
- Desarrollo SQL
- Arquitectura de datos
- Ingeniería de datos
- Desarrollo de pipelines ETL
- Modelado de datos
- Análisis de datos

---

## 🛠️ Enlaces y herramientas importantes:

¡Todo es gratis!

- **[Conjuntos de datos](datasets/):** Acceso al conjunto de datos del proyecto (archivos CSV). - **[SQL Server Express](https://www.microsoft.com/en-us/sql-server/sql-server-downloads):** Servidor ligero para alojar su base de datos SQL.

- **[SQL Server Management Studio (SSMS)](https://learn.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver16):** Interfaz gráfica de usuario (GUI) para administrar e interactuar con bases de datos.

- **[Repositorio Git](https://github.com/):** Configure una cuenta y un repositorio de GitHub para administrar, versionar y colaborar en su código de manera eficiente.

- **[DrawIO](https://www.drawio.com/):** Diseñe arquitecturas de datos, modelos, flujos y diagramas.
- **[Notion](https://www.notion.com/templates/sql-data-warehouse-project):** Obtén la plantilla del proyecto en Notion.
- **[Pasos del proyecto en Notion](https://thankful-pangolin-2ca.notion.site/SQL-Data-Warehouse-Project-16ed041640ef80489667cfe2f380b269?pvs=4):** Acceso a todas las fases y tareas del proyecto.

--

## 🚀 Requisitos del proyecto

### Creación del almacén de datos (Ingeniería de datos)

#### Objetivo
Desarrollar un almacén de datos moderno utilizando SQL Server para consolidar los datos de ventas, lo que permitirá generar informes analíticos y tomar decisiones informadas.

#### Especificaciones
- **Fuentes de datos**: Importar datos de dos sistemas de origen (ERP y CRM) proporcionados como archivos CSV.
- **Calidad de los datos**: Limpiar y resolver los problemas de calidad de los datos antes del análisis.
- **Integración**: Combine ambas fuentes en un único modelo de datos fácil de usar, diseñado para consultas analíticas.
- **Alcance**: Céntrese únicamente en el conjunto de datos más reciente; no se requiere historización de datos.
- **Documentación**: Proporcione documentación clara del modelo de datos para apoyar tanto a las partes interesadas del negocio como a los equipos de análisis.

--

### BI: Análisis e Informes (Análisis de Datos)

#### Objetivo
Desarrollar análisis basados ​​en SQL para proporcionar información detallada sobre:
- **Comportamiento del Cliente**
- **Rendimiento del Producto**
- **Tendencias de Ventas**

Esta información proporciona a las partes interesadas métricas clave del negocio, lo que permite la toma de decisiones estratégicas.

Para obtener más detalles, consulte [docs/requirements.md](docs/requirements.md).

## 📂 Repository Structure
```
data-warehouse-project/
│
├── datasets/                           # Raw datasets used for the project (ERP and CRM data)
│
├── docs/                               # Project documentation and architecture details
│   ├── etl.drawio                      # Draw.io file shows all different techniquies and methods of ETL
│   ├── data_architecture.drawio        # Draw.io file shows the project's architecture
│   ├── data_catalog.md                 # Catalog of datasets, including field descriptions and metadata
│   ├── data_flow.drawio                # Draw.io file for the data flow diagram
│   ├── data_models.drawio              # Draw.io file for data models (star schema)
│   ├── naming-conventions.md           # Consistent naming guidelines for tables, columns, and files
│
├── scripts/                            # SQL scripts for ETL and transformations
│   ├── bronze/                         # Scripts for extracting and loading raw data
│   ├── silver/                         # Scripts for cleaning and transforming data
│   ├── gold/                           # Scripts for creating analytical models
│
├── tests/                              # Test scripts and quality files
│
├── README.md                           # Project overview and instructions
├── LICENSE                             # License information for the repository
├── .gitignore                          # Files and directories to be ignored by Git
└── requirements.txt                    # Dependencies and requirements for the project
```
---
