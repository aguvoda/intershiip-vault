---
tags: [dominio, entidad, company-structure]
---
# AuthorizedSigner · _Firmante autorizado_

Persona autorizada a firmar convenios concretos por una entidad legal o sede.

| Campo | Nota |
|---|---|
| `id`, `legal_entity_id`, `site_id` | |
| `status` | pending \| active \| expired \| revoked |

**MVP:** Parcial — el MVP puede registrar firmante y estado manualmente antes de imponer lógica completa de poderes.

**Relaciones:** [[Entidad - LegalEntity]] · [[Entidad - Site]] · [[Entidad - SignatureRequest]].

Relacionado: [[Modelo de dominio (índice)]] · [[Entidad - SpecificAgreement]]
