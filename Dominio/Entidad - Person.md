---
tags: [dominio, entidad, actor]
---
# Person · _Persona_

> Un ser humano. Puede tener múltiples roles.

Entidad única para cualquier humano. Los roles (alumno, staff, HR, tutor) son asignaciones, no tipos. Una persona puede ser ex-alumno + HR de empresa a la vez — caso real del CETT.

## Campos
| Campo | Tipo | Nota |
|---|---|---|
| `id` | uuid |  |
| `email` | string | único global |
| `full_name` | string |  |
| `avatar_url` | string? |  |
| `phone` | string? |  |
| `linkedin_url` | string? |  |

> [!note] Nota
> NO lleva tenant_id. Las [[Entidad - Membership|Memberships]] la conectan a tenants y roles.

Relacionado: [[Entidad - Membership]] · [[Modelo de dominio (índice)]]
