---
tags: [dominio, entidad, student-access]
---
# Person · _Persona_

Capa de identidad humana que puede conectar varios emails/cuentas en el tiempo. Útil para deduplicación (un ex-alumno que también es HR de empresa — caso real CETT).

| Campo | Nota |
|---|---|
| `id`, `status` | unverified \| merged \| verified |

**MVP:** Parcial — puede mantenerse simple si los imports están controlados. **Dedupe:** email institucional, ID de estudiante, email personal → merge de Person con registros de matrícula específicos.

**Relaciones:** [[Entidad - StudentAccount]] · [[Entidad - UniversityEnrollment]].

Relacionado: [[Modelo de dominio (índice)]]
