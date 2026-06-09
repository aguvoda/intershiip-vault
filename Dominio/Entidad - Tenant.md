---
tags: [dominio, entidad, root]
---
# Tenant · _Centro_

> Una institución educativa. Aislamiento total.

Cada universidad o centro es un tenant. Toda la data (ofertas, alumnos, empresas vinculadas, conversaciones) vive aislada. Las empresas pueden existir en múltiples tenants, pero su relación con cada uno es independiente.

## Campos
| Campo | Tipo | Nota |
|---|---|---|
| `id` | uuid | primary |
| `name` | string | CETT |
| `slug` | string | cett |
| `policy_set_id` | fk → PolicySet | reglas del tenant |
| `lms_integration` | json | config LMS (opcional) |
| `signature_provider` | enum | signaturit | docusign | … |
| `created_at` | timestamp |  |

> [!note] Nota
> Todo query lleva `tenant_id` implícito. Row-level security a nivel DB.

Relacionado: [[Entidad - PolicySet]] · [[Entidad - Membership]] · [[D-03 Empresas globales vs por tenant]] · [[Modelo de dominio (índice)]]
