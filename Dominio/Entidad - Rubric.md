---
tags: [dominio, entidad, document]
---
# Rubric · _Rúbrica_

> Evaluación de prácticas curriculares.

Solo curriculares. Cuestionario que responde la empresa (y opcionalmente el tutor). Su score alimenta la nota exportada al LMS. **Pain #3 de [[Javier (CETT)|Javier]]**.

## Campos
| Campo | Tipo | Nota |
|---|---|---|
| `id` | uuid |  |
| `internship_record_id` | fk → InternshipRecord |  |
| `template_id` | fk → RubricTemplate |  |
| `responses` | json | [{question_id,value,comment}] |
| `company_score` | float? |  |
| `tutor_score` | float? |  |
| `final_grade` | float? |  |
| `submitted_at` | timestamp? |  |
| `lms_sync_status` | enum | pending | synced | failed | manual |
| `lms_synced_at` | timestamp? |  |

Relacionado: [[D-05 LMS push vs pull]] · [[Modelo de dominio (índice)]]
