---
tags: [dominio, entidad, university-structure, mvp]
---
# University · _Universidad / institución_

Entidad institucional padre. Sustituye al `Tenant` genérico v0.2 en el lado universidad.

| Campo | Nota |
|---|---|
| `id`, `name`, `legal_name`, `domain`, `country` | |
| `account_status` | limited \| active \| suspended \| churned |
| `plan_status` | School / Institution / University Pro / Enterprise ([[Pricing]]) |

> [!note] Una universidad **invitada por una empresa** puede existir como `limited` antes de ser de pago (entra por el flywheel). Ver [[Cuentas, roles y trust levels]].

**Dedupe:** domain, nombre oficial, país/ciudad → merge solo por admin.

**Relaciones:** [[Entidad - AcademicUnit]] · Account · [[Entidad - ReferralLead]] · [[Entidad - InstitutionalRelationship]]. **MVP:** Sí.

Relacionado: [[Modelo de dominio (índice)]] · [[Tesis 3 - Diseñar desde la universidad más compleja]]
