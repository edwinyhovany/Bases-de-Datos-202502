# Proyecto de Gestión Académica (Examen Final SQL & Pandas)

Este proyecto contiene el desarrollo del primer examen práctico para la asignatura de Bases de Datos, enfocado en la manipulación y análisis de datos de un sistema académico universitario utilizando SQLite y la biblioteca Pandas.

## Objetivo del Proyecto

El objetivo principal es demostrar la competencia en las siguientes áreas:

1.  **Manipulación de Datos (DML):** Realizar operaciones de inserción, actualización y eliminación (`INSERT`, `UPDATE`, `DELETE`) para gestionar registros académicos (apertura de cursos, matrícula, y retiro de estudiantes).
2.  **Consultas (SELECT):** Construir consultas `JOIN` y de agregación (`AVG`, `COUNT`, `GROUP BY`) para extraer métricas clave del sistema.
3.  **Analítica con Python (Pandas & Matplotlib):** Cargar los datos a un DataFrame, limpiar valores nulos y generar reportes avanzados (Tablas Pivote, Distribución de Notas y Análisis de Riesgo).

## Contenido del Repositorio

| Archivo/Carpeta | Descripción |
| :---: | :--- |
| **`universidad.db`** | Base de datos SQLite que contiene las tablas: `Estudiantes`, `Profesores`, `Cursos`, e `Inscripciones` |
| **`Examen1.ipynb`** | Cuaderno de Jupyter/VS Code que contiene el desarrollo completo del examen, desde la configuración inicial hasta la generación de gráficos|
| **`README_DB.md`** | Descripción detallada de la estructura de la base de datos (este archivo) |

## Requisitos y Ejecución

### Requisitos de Software

Para ejecutar el cuaderno, se debe tener instalado:

* **Python 3.x**
* **Jupyter Notebook** (o la extensión Jupyter en VS Code)
* **Bibliotecas de Python:**
    * `sqlite3` (Generalmente incluida en Python)
    * `pandas`
    * `matplotlib`

## Pasos para la Ejecución

Para iniciar el proyecto y ejecutar el examen completo, sigue estos pasos secuenciales:

1.  **Clonar o Descargar** este proyecto en tu sistema local.
2.  **Verificación de Ruta:** Asegúrate de que el archivo de base de datos **`universidad.db`** esté en la misma carpeta que el cuaderno **`Examen1.ipynb`**.
3.  **Apertura del Cuaderno:** Abre el archivo **`Examen1.ipynb`** usando Visual Studio Code, Jupyter Notebook, o Google Colab.
4.  **Configuración Inicial:** Ejecuta la primera celda (`CONFIGURACIÓN INICIAL`) para **establecer la conexión** (`conn` y `cursor`) con la base de datos.
5.  **Sección 1 (DML):** Ejecuta secuencialmente las celdas de la **Sección 1** para realizar las modificaciones de registros (`INSERT`, `UPDATE`, `DELETE`) en las tablas.
6.  **Sección 2 (SELECT):** Ejecuta las celdas de la **Sección 2** para obtener los datos de análisis mediante consultas `SELECT` (Puntos 6 al 11).
7.  **Sección 3 (Pandas):** Ejecuta las celdas de la **Sección 3** para cargar el `DataFrame` y generar los reportes analíticos y visualizaciones finales (Puntos 13, 14, 15).

