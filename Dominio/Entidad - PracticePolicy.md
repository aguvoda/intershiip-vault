---
tags: [dominio, entidad, university-structure, mvp]
---
# PracticePolicy · _Política de prácticas_

Reglas para prácticas por universidad, unidad académica o programa. Sustituye a `PolicySet` v0.2. Sigue siendo **reglas como datos, no hardcode** ([[Capa - Policy layer]]).

| Campo | Nota |
|---|---|
| `id`, scope (`academic_program_id` / unit / university) | |
| `status` | draft \| active \| archived |

> [!note] Jerarquía de override
> Política de **programa** sobreescribe la de **unidad académica**, que sobreescribe la de **universidad**.

**Relaciones:** [[Entidad - AcademicProgram]] · AgreementCoverage · [[Entidad - PracticeCase]]. **MVP:** Sí, simplificado.

Relacionado: [[Capa - Policy layer]] · [[D-06 Convenio curricular + extracurricular]]
