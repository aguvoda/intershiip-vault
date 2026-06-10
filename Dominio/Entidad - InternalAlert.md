---
tags: [dominio, entidad, network-activation, mvp]
---
# InternalAlert · _Alerta interna_

Notificación accionable al equipo de Internshiip para **hot leads** y riesgos operativos.

| Campo | Nota |
|---|---|
| `id`, `alert_type`, `entity_type`, `entity_id`, `priority` | |
| `owner_user_id`, `status` (new → acknowledged → in_progress → resolved / dismissed) | |
| `created_at`, `resolved_at` | |

> [!note] **"Empresa recomienda universidad"** debe dispararla de inmediato (obligatoria al `ReferralLead.submitted`). Si no, se pierde la venta.

**Relaciones:** [[Entidad - ReferralLead]] · [[Entidad - CompanyInterest]] · [[Entidad - PracticeCase]] · [[Entidad - SuccessFeeEvent]]. **MVP:** Sí.

Relacionado: [[Relationship flywheel]] · [[Modelo de dominio (índice)]]
