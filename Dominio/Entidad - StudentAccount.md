---
tags: [dominio, entidad, student-access, mvp]
---
# StudentAccount · _Cuenta de alumno_

Login/perfil de un alumno o candidato. Sustituye a `StudentProfile` v0.2.

| Campo | Nota |
|---|---|
| `id`, `person_id`, `login_email`, `created_at` | |
| `status` | self_registered → email_verified → institution_pending_verification → institution_verified → alumni · *otros:* rejected_by_institution / deleted |

> [!warning] Perfil libre, práctica verificada
> El auto-registro está permitido. La **candidatura formal NO se permite sin verificación institucional** ([[Entidad - UniversityEnrollment]]). Sin verificar solo puede [[Entidad - StudentInterest|expresar interés]].

**Relaciones:** [[Entidad - UniversityEnrollment]] · [[Entidad - StudentInterest]] · [[Entidad - Application]]. **MVP:** Sí.

Relacionado: [[Cuentas, roles y trust levels]] · [[Capa - State machine]]
