#  Estructura de la Base de Datos: Universidad Santo Tomás

Este documento describe la estructura de la base de datos `universidad.db`, la cual simula el sistema de gestión académica de una universidad.

##  Tablas y Descripción

| Tabla | Descripción | Clave Primaria (PK) | Relaciones (FK) |
| :---: | :---: | :---: | :---: |
| **Estudiantes** | Almacena la información personal de cada estudiante activo en el sistema. | `id_estudiante` | - |
| **Profesores** | Almacena la información de los docentes que dictan los cursos. | `id_profesor` | - |
| **Cursos** | Lista de cursos ofrecidos, incluyendo créditos y el docente responsable. | `id_curso` | `id_profesor` (FK a Profesores) |
| **Inscripciones** | Tabla central (muchos a muchos) que registra la matrícula de un estudiante en un curso y su calificación final. | Compuesta: (`id_estudiante`, `id_curso`) | `id_estudiante` (FK a Estudiantes), `id_curso` (FK a Cursos) |

---

## Reglas de Integridad (Claves Foráneas)

Las siguientes restricciones de clave foránea garantizan la coherencia de los datos en el sistema:

1.  **Cursos ➡️ Profesores:** Cada curso debe estar asignado a un profesor existente.
2.  **Inscripciones ➡️ Estudiantes:** Cada inscripción debe pertenecer a un estudiante existente.
3.  **Inscripciones ➡️ Cursos:** Cada inscripción debe corresponder a un curso ofertado existente.

**Nota:** La tabla `Inscripciones` está configurada con una restricción `UNIQUE` en la combinación de `(id_estudiante, id_curso)` para evitar que un estudiante se matricule dos veces en la misma materia.

---

## Observaciones 

* Se observa que la columna `nota_final` en la tabla `Inscripciones` contiene inicialmente valores nulos (`NULL`) que deben ser tratados y asignados mediante comandos DML y técnicas de análisis.
