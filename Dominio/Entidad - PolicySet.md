---
tags: [dominio, entidad, governance]
---
# PolicySet · _Normativa_

> Reglas del tenant como datos.

Validaciones, mínimos legales, plantillas de convenio, campos obligatorios, horas por programa, reglas de firma. Versionado — cada [[Entidad - InternshipRecord|InternshipRecord]] lleva un snapshot de la política vigente al crearse.

## Campos
| Campo | Tipo | Nota |
|---|---|---|
| `id` | uuid |  |
| `tenant_id` | fk → Tenant |  |
| `version` | int |  |
| `rules` | json | DSL declarativo |
| `active_from` | date |  |
| `active_to` | date? |  |

Relacionado: [[Capa - Policy layer]] · [[Modelo de dominio (índice)]]
