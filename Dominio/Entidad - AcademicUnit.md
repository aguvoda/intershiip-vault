---
tags: [dominio, entidad, university-structure, mvp]
---
# AcademicUnit · _Unidad académica_

Facultad, escuela, centro, campus, departamento o unidad anidada. Es la base del **modelo de scopes** (un coordinador de Economía no debería ver Derecho).

| Campo | Nota |
|---|---|
| `id`, `university_id`, `parent_academic_unit_id` | jerarquía anidada |
| `type`, `name`, `status` (active/inactive) | |

> [!note] Debe soportar jerarquía: University → AcademicUnit → AcademicUnit hija → AcademicProgram.

**Relaciones:** [[Entidad - University]] · [[Entidad - AcademicProgram]] · [[Entidad - PracticePolicy]] · [[Entidad - InstitutionalPosting]]. **MVP:** Sí.

Relacionado: [[Cuentas, roles y trust levels]] · [[D-02 Tutor rol global vs por programa]]
