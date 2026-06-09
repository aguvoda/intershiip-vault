---
tags: [dominio, entidad, document]
---
# Document · _Documento_

> Archivo versionado.

Archivo binario (PDF, imagen, doc). Versionado, con checksum. Referenciado desde múltiples entidades (CV, convenio, adjunto).

## Campos
| Campo | Tipo | Nota |
|---|---|---|
| `id` | uuid |  |
| `tenant_id` | fk → Tenant |  |
| `kind` | enum | cv | agreement | attachment | rubric_export | audit_pack |
| `filename` | string |  |
| `mime_type` | string |  |
| `size_bytes` | int |  |
| `checksum` | string | sha256 |
| `version` | int |  |
| `storage_ref` | string | s3://… |

Relacionado: [[Entidad - Agreement]] · [[Modelo de dominio (índice)]]
