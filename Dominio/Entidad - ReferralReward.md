---
tags: [dominio, entidad, revenue-reward, mvp]
---
# ReferralReward · _Recompensa por referral_

Descuento o crédito que gana un referrer cuando se cumple el disparador. **La recompensa no se gana por recomendar; se gana cuando la recomendación convierte.**

| Campo | Nota |
|---|---|
| `id`, `referral_lead_id`, `beneficiary_actor_type/id`, `trigger_event`, `reward_type`, `reward_value` | |
| `status` | pending → earned → applied · *otros:* expired / cancelled / disputed |

| Referral | Beneficiario | Disparador |
|---|---|---|
| Empresa recomienda universidad | Empresa | universidad pasa a **pago** |
| Universidad importa empresa | Universidad | primera práctica **firmada** |
| Cadena indirecta | solo referrer directo (MVP) | evita compensación multinivel |

**Relaciones:** [[Entidad - ReferralLead]] · [[Entidad - SuccessFeeEvent]] · Account. **MVP:** Sí, mínimo.

Relacionado: [[Relationship flywheel]] · [[Modelo de monetización]]
