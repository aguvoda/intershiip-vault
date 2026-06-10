---
tags: [dominio, entidad, student-access, mvp]
---
# StudentInterest · _Interés de alumno_

Interés **no formal** en una oportunidad por un alumno no verificado o aún no elegible. Captura demanda sin crear candidaturas inválidas/ilegales.

| Campo | Nota |
|---|---|
| `id`, `student_account_id`, `master_opportunity_id`, `university_id`, `created_at` | |
| `status` | saved \| requested_access \| converted_to_application \| expired |

> [!note] Discovery puede ser público; la aplicación formal exige verificación institucional. Si la universidad no está conectada → StudentDemandLead / activation request (señal de demanda agregada).

**Relaciones:** [[Entidad - StudentAccount]] · [[Entidad - MasterOpportunity]] · [[Entidad - University]]. **MVP:** Sí.

Relacionado: [[Modelo de dominio (índice)]] · [[Tesis 5 - Voice-First Student Experience]]
