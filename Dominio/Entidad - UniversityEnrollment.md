---
tags: [dominio, entidad, student-access, mvp]
---
# UniversityEnrollment · _Matrícula_

Relación verificada (o pendiente) entre un alumno y una universidad/programa. **Fuente de verdad de la elegibilidad** para prácticas formales.

| Campo | Nota |
|---|---|
| `id`, `student_account_id`, `university_id`, `academic_unit_id`, `academic_program_id` | |
| `verification_status` | pending \| verified \| rejected \| expired \| alumni |

> [!note] La controla la **universidad**, no el alumno auto-registrado. En MVP: import/validación manual de la universidad; futuro: integración SIS.

**Relaciones:** [[Entidad - StudentAccount]] · [[Entidad - University]] · [[Entidad - AcademicProgram]] · [[Entidad - PracticeCase]]. **MVP:** Sí.

Relacionado: [[Modelo de dominio (índice)]] · [[Cuentas, roles y trust levels]]
