---
tags: [dominio, entidad, opportunity-distribution, core, mvp]
---
# InstitutionalPosting · _Publicación institucional_

Versión específica de una [[Entidad - MasterOpportunity|MasterOpportunity]] **gobernada por la universidad/centro**. Protege el sentido de propiedad y control de la institución — no es un listado de marketplace.

| Campo | Nota |
|---|---|
| `id`, `master_opportunity_id`, `university_id`, `academic_unit_id`, `academic_program_id` | |
| `status` | draft → under_review → needs_changes → published → applications_open → closed · *otros:* rejected / cancelled |
| `visibility_mode` | private_institutional \| shared_selected \| public_preview \| (public_open: evitar en MVP) |

> [!note] La universidad personaliza programas elegibles, requisitos, texto al alumno y reglas de aplicación. El alumno ve **su** tablón, no un marketplace genérico.

**Relaciones:** [[Entidad - MasterOpportunity]] · [[Entidad - AcademicUnit]] · [[Entidad - AcademicProgram]] · [[Entidad - Application]]. **MVP:** Sí.

Relacionado: [[Distribución MasterOpportunity vs InstitutionalPosting]] · [[Capa - State machine]]
