---
tags: [dominio, entidad, core]
---
# Opportunity · _Oferta_

> [!check] Decisión D-01 (2026-06-09)
> **Opportunity es una entidad única = "una oferta". Sin subtipos** (se descartan `job/internship/tfg/challenge`). Es la **puerta de entrada** del sistema. Ver [[D-01 Opportunity polimórfica]].

Una empresa publica una **oferta de prácticas** para los alumnos de un centro. Es la entidad madre del flujo: cuando un alumno es aceptado en una oferta, nace un [[Entidad - InternshipRecord|InternshipRecord]].

## Campos
| Campo | Tipo | Nota |
|---|---|---|
| `id` | uuid | OPP-2026-0347 |
| `tenant_id` | fk → Tenant | |
| `organization_id` | fk → Organization | |
| `created_by_membership_id` | fk → Membership | HR que publicó |
| `title` | string | |
| `description` | markdown | |
| `location` | json | {city, remote, hybrid} |
| `compensation` | json? | {amount, currency, period} |
| `target_programs` | fk[] | AcademicProgram (visibilidad) |
| `modality` | enum | curricular \| extracurricular \| **mixed** |
| `hours_range` | json | {min, max} |
| `status` | enum | draft \| pending_review \| open \| closed \| archived |
| `published_at` | timestamp? | |
| `expires_at` | timestamp? | |

> [!note] Flujo
> Hay **un único flujo de publicación** de ofertas. Una oferta recibe [[Entidad - Application|candidaturas]]; al aceptar una, se genera el [[Entidad - InternshipRecord|expediente]].

Relacionado: [[Entidad - Application]] · [[Entidad - InternshipRecord]] · [[D-06 Convenio curricular + extracurricular]] · [[Modelo de dominio (índice)]]
