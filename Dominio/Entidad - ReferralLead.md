---
tags: [dominio, entidad, network-activation, core, mvp]
---
# ReferralLead · _Lead de relación_

> [!info] Entidad de crecimiento central
> Toda señal de relación entrante (import, referral de empresa, interés) debe convertirse en un lead o en un evento de actividad. Tiene **fuente y target claros**.

| Campo | Nota |
|---|---|
| `id`, `referrer_actor_type/id` | quién lo origina |
| `target_actor_type`, `target_name`, `target_contact_id` | |
| `source_channel`, `assigned_owner_user_id` | |
| `status` | submitted → pending_review → approved → invited → opened → accepted → registered_limited → sales_qualified → converted_paid · *salidas:* rejected / expired / duplicate / opted_out |

**Dedupe:** target institución/contacto + ventana → primer referrer válido gana **90 días**; conflicto estratégico = revisión manual.

**Relaciones:** [[Entidad - Invitation]] · [[Entidad - ReferralReward]] · [[Entidad - InstitutionalRelationship]] · [[Entidad - AttributionEvent]]. **MVP:** Sí.

Relacionado: [[Relationship flywheel]] · [[Modelo de monetización]] · [[Capa - State machine]]
