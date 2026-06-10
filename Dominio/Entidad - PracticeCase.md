---
tags: [dominio, entidad, practice-operations, core, mvp]
---
# PracticeCase · _Expediente de prácticas_

> [!info] Ancla de monetización y compliance
> Expediente legal-operativo creado desde una [[Entidad - Application|Application]] seleccionada. Sustituye a `InternshipRecord` v0.2. Es lo que hace el modelo defendible y monetizable.

| Campo | Nota |
|---|---|
| `id`, `application_id`, `student_id`, `university_id`, `organization_id` | |
| `start_date`, `end_date`, `hours` | |
| `status` | created → eligibility_pending → agreement_draft → signature_pending → fully_signed → prestart_checklist_pending → ready_to_start → in_progress → completed → closed · *salidas:* eligibility_failed / prestart_blocked / cancelled / early_terminated |

**Stage lineal, readiness paralelo:** el expediente avanza en una fase principal, pero firmas, seguro, tutor, horas, fechas y elegibilidad avanzan en paralelo ([[Entidad - PreStartChecklist]]).

**Relaciones:** [[Entidad - Application]] · [[Entidad - SpecificAgreement]] · [[Entidad - SuccessFeeEvent]] · [[Entidad - StudentAccount]] · [[Entidad - Organization]]. **MVP:** Sí.

Relacionado: [[Capa - State machine]] · [[Modelo de monetización]] · [[D-06 Convenio curricular + extracurricular]]
