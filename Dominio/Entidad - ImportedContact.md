---
tags: [dominio, entidad, network-activation, mvp]
---
# ImportedContact · _Contacto importado_

Una fila de contacto de un import, antes o después de deduplicar.

| Campo | Nota |
|---|---|
| `id`, `contact_import_id` | |
| `name`, `email`, `phone`, `role_title`, `organization_name` | |
| `relationship_context` | contexto de la relación (compliance) |
| `status` | raw \| mapped \| duplicate \| valid \| needs_review \| do_not_contact |
| `opt_out_status` | |

> [!note] Debe preservar **fuente, contexto de relación y opt-out**. Los estados do-not-contact / bounced / wrong-person / opted-out son de sistema, no notas sueltas.

**Relaciones:** [[Entidad - ContactImport]] · [[Entidad - InstitutionContact]] · [[Entidad - ReferralLead]]. **MVP:** Sí.

Relacionado: [[Modelo de dominio (índice)]] · [[Cumplimiento y datos (compliance)]]
