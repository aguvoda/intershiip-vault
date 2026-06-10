---
tags: [dominio, entidad, network-activation, mvp]
---
# ContactImport · _Lote de contactos_

Lote de contactos subido por una universidad, empresa o admin de Internshiip. Es el inicio del flywheel: la universidad activa su red existente.

| Campo | Nota |
|---|---|
| `id`, `source_actor_type`, `source_actor_id` | quién sube |
| `uploaded_by_user_id`, `file_name`, `created_at` | |
| `status` | uploaded → mapped → deduped → reviewed → processed / failed |

> [!warning] Regla
> **Importar nunca envía invitaciones automáticamente.** Siempre hay paso de revisión/aprobación. Ver [[Cumplimiento y datos (compliance)]].

**Relaciones:** [[Entidad - ImportedContact]] · [[Entidad - AttributionEvent]] · [[Entidad - ReferralLead]]. **MVP:** Sí.

Relacionado: [[Modelo de dominio (índice)]] · [[Relationship flywheel]]
