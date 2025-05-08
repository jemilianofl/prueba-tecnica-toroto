# 📊 Solución al Challenge de Innovación 2025 - Toroto

Este proyecto fue desarrollado como parte del reto técnico propuesto en el Challenge de Innovación 2025. Tiene como objetivo brindar una solución completa e integrada para la visualización, integración y automatización de datos de obras, mejorando la eficiencia operativa, la digitalización y el análisis de la información de campo.

---
# 🚀 Objetivo del Proyecto

Desarrollar un sistema que automatice la carga de datos de obras desde archivos Excel hacia una base de datos estructurada, sincronice dicha información con herramientas colaborativas [Coda.io](https://coda.io/developers/apis/v1#) y presente visualizaciones analíticas interactivas para toma de decisiones.

---
# 🧩 Componentes de la Solución

🔹 Parte 1: Ingesta de Datos a Supabase

- Lectura y normalización de un archivo Excel.

- Inserción de datos en PostgreSQL (Supabase) usando SQLAlchemy ORM.

- Tablas utilizadas: proyectos, cuadrillas, responsables, obras, evidencias.

**Motivo**: automatizar el paso inicial de carga de datos sin errores manuales y de forma estructurada.

🔹 Parte 2: Sincronización con [Coda.io](https://coda.io/developers/apis/v1#)

- Extracción de datos desde Supabase con ORM.

- Serialización e inserción de bloques de datos en una tabla de Coda usando su API.

- Manejo de rate limits (429 Too Many Requests) con reintentos y espera exponencial.

**Motivo**: mantener sincronizada la información en herramientas colaborativas que usa el equipo operativo.

🔹 Parte 3: Dashboard Analítico con Streamlit

- Consultas agrupadas por proyecto y cuadrilla usando ORM.

- Visualización con Plotly de datos agrupados por tipo de obra.

- Interfaz moderna con modo oscuro y estilo corporativo.

**Motivo**: facilitar el análisis visual de los datos para usuarios no técnicos, permitiendo una mejor planeación y seguimiento.

---
# 📂 Tecnologías utilizadas

| Herramienta | Uso principal |
|----------|----------|
| Python               | Lógica de negocio y procesamiento |
| SQLAlchemy | ORM para interactuar con la base de datos   |
| PostgreSQL (Railway) | Almacenamiento de datos estructurados   |
| Streamlit              | Dashboard interactivo |
| Plotly | ORM para interactuar con la base de datos   |
| Coda API    | Integración con herramientas colaborativas   |
| Docker + Railway    | Contenedorización y despliegue web   |

---
# 📈 Beneficios

- 🔄 Automatización del flujo de datos desde Excel hasta herramientas web.

- 📉 Reducción de errores humanos y duplicidad de datos.

- 🧠 Visualizaciones interactivas para facilitar el análisis técnico y operativo.

- 🌐 Accesible desde la nube por cualquier miembro del equipo.

# Nuevas Funcionalidades
- Se agregaron nuevas carpetas con el sufijo Railway debido a migración del servicio completo a Railway, esto por el despliegue de las aplicaciones y redireccion de los servicios.
- Pueden acceder al [Dashboard en:](toroto-parte03-railway-production.up.railway.app)