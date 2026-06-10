---
tags: [dominio, entidad, network-activation, core, mvp]
---
# AttributionEvent · _Evento de atribución_

Registro **append-only** de fuente, actor, evento y target. Columna vertebral para crecimiento, billing, rewards y auditoría. Sustituye a la entidad `Event` v0.2.

| Campo | Nota |
|---|---|
| `id`, `entity_type`, `entity_id`, `event_type` | |
| `source_actor_type/id`, `source_user_id`, `metadata`, `created_at` | |

> [!important] Append-only desde el MVP
> Nunca se sobreescribe. Aunque el resto del modelo cambie, atribución, billing y compliance dependen del historial de eventos. No confiar solo en campos actuales: reconstruir la historia desde eventos. Registra: quién subió un contacto, quién aprobó una invitación, cuándo una MasterOpportunity pasó a InstitutionalPosting, cuándo un SpecificAgreement quedó fully_signed y qué SuccessFeeEvent generó.

**Relaciones:** todas las entidades de lead, account, posting, firma y reward. **MVP:** Sí.

Relacionado: [[Capa - Event log]] · [[Modelo de monetización]] · [[Cuentas, roles y trust levels]]
