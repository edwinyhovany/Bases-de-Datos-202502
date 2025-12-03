# Proyecto de Gestión Académica (Examen Final SQL & Pandas)

Este proyecto contiene el desarrollo del examen final práctico para la asignatura de Bases de Datos, enfocado en la manipulación y análisis de datos de un sistema académico universitario utilizando SQLite y la biblioteca Pandas.

## Objetivo del Proyecto

El objetivo principal es demostrar la competencia en las siguientes áreas:

1.  **Manipulación de Datos (DML):** Realizar operaciones de inserción, actualización y eliminación (`INSERT`, `UPDATE`, `DELETE`) para gestionar registros académicos (apertura de cursos, matrícula, y retiro de estudiantes).
2.  **Consultas (SELECT):** Construir consultas `JOIN` y de agregación (`AVG`, `COUNT`, `GROUP BY`) para extraer métricas clave del sistema.
3.  **Analítica con Python (Pandas & Matplotlib):** Cargar los datos a un DataFrame, limpiar valores nulos y generar reportes avanzados (Tablas Pivote, Distribución de Notas y Análisis de Riesgo).

## Contenido del Repositorio

| Archivo/Carpeta | Descripción |
| :---: | :--- |
| **`universidad.db`** | Base de datos SQLite que contiene las tablas: `Estudiantes`, `Profesores`, `Cursos`, e `Inscripciones`. |
| **`Examen (1).ipynb`** | Cuaderno de Jupyter/VS Code que contiene el desarrollo completo del examen, desde la configuración inicial hasta la generación de gráficos. |
| **`README_DB.md`** | Descripción detallada de la estructura de la base de datos (este archivo). |

## Requisitos y Ejecución

### Requisitos de Software

Para ejecutar el cuaderno, se debe tener instalado:

* **Python 3.x**
* **Jupyter Notebook** (o la extensión Jupyter en VS Code)
* **Bibliotecas de Python:**
    * `sqlite3` (Generalmente incluida en Python)
    * `pandas`
    * `matplotlib`

Puede instalar las bibliotecas necesarias usando pip:
```bash
pip install pandas matplotlib
