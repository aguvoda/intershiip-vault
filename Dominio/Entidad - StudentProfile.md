---
tags: [dominio, entidad, actor]
---
# StudentProfile · _Perfil de alumno_

> Personal branding + expectativas.

CV, intereses, expectativas (horario, sector, funciones, horas, modalidad). Las expectativas alimentan la casación asistida — **pain #1 de [[Javier (CETT)|Javier]]**.

## Campos
| Campo | Tipo | Nota |
|---|---|---|
| `id` | uuid |  |
| `membership_id` | fk → Membership | rol=student |
| `program_id` | fk → AcademicProgram |  |
| `cohort_year` | int | 2025 |
| `bio` | markdown |  |
| `cv_document_id` | fk → Document? |  |
| `skills` | string[] |  |
| `languages` | json | [{code,level}] |
| `expectations` | json | {hours,schedule,sectors,functions,modality,location} |
| `availability` | json | desde/hasta, horas/semana |
| `visible_to_companies` | boolean |  |

> [!note] Nota
> `expectations` es el campo clave: drive del matching.

Relacionado: [[Entidad - Application]] · [[Modelo de dominio (índice)]]
