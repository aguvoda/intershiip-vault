---
tags: [dominio, entidad, university-structure, mvp]
---
# AcademicProgram · _Programa académico_

Grado, máster, postgrado o programa de FP. El scope de programa es necesario para coverage, elegibilidad y targeting de publicaciones.

| Campo | Nota |
|---|---|
| `id`, `university_id`, `academic_unit_id` | |
| `name`, `level` (bachelor/master/vocational/dual), `status` | |
| `min_curricular_hours`, `max_extracurricular_hours`, `requires_evaluation` | requisitos de prácticas por programa |

**Relaciones:** [[Entidad - AcademicUnit]] · [[Entidad - PracticePolicy]] · [[Entidad - InstitutionalPosting]] · [[Entidad - UniversityEnrollment]]. **MVP:** Sí.

Relacionado: [[Modelo de dominio (índice)]] · [[D-02 Tutor rol global vs por programa]] · [[D-06 Convenio curricular + extracurricular]] · [[D-09 Formación dual]]
