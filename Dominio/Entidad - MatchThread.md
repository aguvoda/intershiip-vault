---
tags: [dominio, entidad, core]
---
# MatchThread · _Trayecto de candidaturas_

> [!check] Decisión D-04 (2026-06-09)
> **Aprobada.** Agrupa **todas las candidaturas de un alumno** (todas las [[Entidad - Opportunity|ofertas]] a las que aplicó) para ver su trayecto en un solo sitio. Ver [[D-04 Application por intento vs MatchThread]].

Contenedor que reúne las [[Entidad - Application|Applications]] de un alumno. Resuelve el caso real de prospección dirigida (un alumno enviado a muchas empresas): cada envío sigue siendo una Application atómica, pero el MatchThread da la **vista de campaña / trayecto completo**.

## Campos
| Campo | Tipo | Nota |
|---|---|---|
| `id` | uuid | |
| `tenant_id` | fk → Tenant | |
| `student_profile_id` | fk → StudentProfile | de quién es el trayecto |
| `managed_by_membership_id` | fk → Membership? | Career Service que lo gestiona |
| `title` | string? | ej. "Búsqueda prácticas 2026" |
| `status` | enum | active \| closed |
| `created_at` | timestamp | |

> [!note] Nota
> Una Application puede pertenecer a un MatchThread (`match_thread_id`). Vista pensada para Career Service.

Relacionado: [[Entidad - Application]] · [[Entidad - StudentProfile]] · [[Modelo de dominio (índice)]]
