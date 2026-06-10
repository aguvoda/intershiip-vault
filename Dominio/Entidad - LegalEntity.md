---
tags: [dominio, entidad, company-structure, mvp]
---
# LegalEntity · _Entidad legal_

Entidad con identificación fiscal (CIF/NIF) que **puede firmar convenios**. Una [[Entidad - Organization|Organization]] puede tener varias.

| Campo | Nota |
|---|---|
| `id`, `organization_id`, `legal_name`, `tax_id`, `country` | |
| `status` | active \| inactive |

**Relaciones:** [[Entidad - Organization]] · [[Entidad - Site]] · FrameworkAgreement · [[Entidad - SpecificAgreement]]. **MVP:** Sí, simplificado.

Relacionado: [[Modelo de dominio (índice)]] · [[Entidad - AuthorizedSigner]]
