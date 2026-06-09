---
tags: [dominio, entidad, context]
---
# AcademicProgram · _Titulación_

> Un grado, máster o ciclo.

Qué grados ofrece el tenant, requisitos de prácticas por programa, min/max horas curriculares y extracurriculares, qué asignaturas son practicum.

## Campos
| Campo | Tipo | Nota |
|---|---|---|
| `id` | uuid |  |
| `tenant_id` | fk → Tenant |  |
| `name` | string | Grado en Dirección Hotelera |
| `kind` | enum | bachelor | master | vocational | dual |
| `min_curricular_hours` | int | 250 |
| `max_extracurricular_hours` | int | 900 |
| `requires_rubric` | boolean |  |
| `practicum_course_id` | string? | ID LMS |

Relacionado: [[D-06 Convenio curricular + extracurricular]] · [[D-09 Formación dual]] · [[Modelo de dominio (índice)]]
