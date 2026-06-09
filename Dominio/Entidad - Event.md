---
tags: [dominio, entidad, spine]
---
# Event · _Evento del sistema_

> Log inmutable. La espina del sistema.

Cada acción relevante genera un evento. **Append-only.** Hace auditable el sistema y permite reconstruir cualquier estado. Alimenta notificaciones, métricas y agent layer.

## Campos
| Campo | Tipo | Nota |
|---|---|---|
| `id` | uuid |  |
| `tenant_id` | fk → Tenant |  |
| `ts` | timestamp |  |
| `type` | string | agreement.signed_by_company |
| `actor_membership_id` | fk → Membership? |  |
| `actor_kind` | enum | human | system | agent |
| `entity_type` | string | InternshipRecord |
| `entity_id` | uuid |  |
| `payload` | json |  |

> [!note] Nota
> Nunca UPDATE. Solo INSERT. Los cambios se expresan como nuevo evento.

Relacionado: [[Capa - Event log]] · [[Modelo de dominio (índice)]]
