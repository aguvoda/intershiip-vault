---
tags: [dominio, entidad, student-access, core, mvp]
---
# Application · _Candidatura_

Candidatura formal o candidato propuesto por la universidad para una [[Entidad - InstitutionalPosting|InstitutionalPosting]]. **Solo alumnos verificados** crean candidaturas formales a prácticas institucionales.

| Campo | Nota |
|---|---|
| `id`, `institutional_posting_id`, `student_account_id` | |
| `source` | applied \| suggested (propuesto por universidad) |
| `status` | applied / suggested → under_review → interview_pending → selected / rejected / withdrawn / expired |
| `selected_at`, `rejected_reason` | |

> [!note] Al `selected`, una candidatura crea un [[Entidad - PracticeCase|PracticeCase]]. El interés no formal vive en [[Entidad - StudentInterest|StudentInterest]] (no es Application).

**Relaciones:** [[Entidad - InstitutionalPosting]] · [[Entidad - StudentAccount]] · [[Entidad - PracticeCase]]. **MVP:** Sí.

Relacionado: [[Entidad - StudentInterest]] · [[Modelo de dominio (índice)]]
