---
tags: [dominio, entidad, document]
---
# Agreement · _Convenio_

> El convenio firmado. Versionado.

Documento legal vinculante, generado desde plantilla del tenant. Versionado (cada revisión = nuevo doc). Integra con proveedor de firma (Signaturit).

## Campos
| Campo | Tipo | Nota |
|---|---|---|
| `id` | uuid |  |
| `internship_record_id` | fk → InternshipRecord |  |
| `template_id` | fk → AgreementTemplate |  |
| `version` | int | 1,2,3… |
| `status` | enum | draft | sent | partially_signed | signed | void |
| `signatures` | json | [{party,signed_at,ip}] |
| `document_id` | fk → Document | PDF generado |
| `signature_provider_ref` | string? | ID Signaturit |

Relacionado: [[Agente - Agreement Coordinator]] · [[Modelo de dominio (índice)]]
