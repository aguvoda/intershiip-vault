---
tags: [dominio, entidad, network-activation, mvp]
---
# Invitation · _Invitación_

Invitación concreta enviada a un contacto o email institucional. El copy debe ser **contextual** ("CETT te ha invitado a gestionar prácticas con sus alumnos"), nunca spam genérico de plataforma.

| Campo | Nota |
|---|---|
| `id`, `referral_lead_id`, `recipient_email`, `template_id` | |
| `sender_context`, `legal_basis_tag`, `opt_out_link` | compliance |
| `status` | draft → scheduled → sent → opened → clicked → accepted / declined / bounced / opted_out |
| `sent_at`, `opened_at`, `accepted_at`, `bounced_at` | |

**Relaciones:** [[Entidad - ReferralLead]] · [[Entidad - InstitutionContact]] · Account. **MVP:** Sí.

Relacionado: [[Modelo de dominio (índice)]] · [[Cumplimiento y datos (compliance)]]
