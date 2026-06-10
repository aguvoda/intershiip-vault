---
tags: [dominio, entidad, practice-operations, mvp]
---
# SignatureRequest / SignatureStatus · _Firma_

Estado de firma para los actores empresa, universidad y alumno (firman **por separado**).

| Campo | Nota |
|---|---|
| `id`, `specific_agreement_id` | |
| `status` | pending \| sent \| viewed \| signed \| declined \| expired \| manually_uploaded |

> [!note] MVP: estado **manual** antes de integrar proveedores de firma. No mina el disparador de fee mientras el estado sea fiable.

**Relaciones:** [[Entidad - SpecificAgreement]] · [[Entidad - AuthorizedSigner]]. **MVP:** Sí, mínimo.

Relacionado: [[Modelo de dominio (índice)]] · [[D-05 LMS push vs pull]]
