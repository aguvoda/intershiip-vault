---
tags: [dominio, entidad, actor]
---
# Membership · _Vínculo_

> [!check] Decisión D-02 (2026-06-09)
> El **tutor se asigna por programa**, no como rol global con delegación. `TutorDelegation` queda descartado. Ver [[D-02 Tutor rol global vs por programa]].

> Persona × Tenant × Rol.

Conecta Person con Tenant y le asigna un rol. Una persona puede tener varias memberships. Los permisos se derivan de aquí.

## Campos
| Campo | Tipo | Nota |
|---|---|---|
| `id` | uuid |  |
| `tenant_id` | fk → Tenant |  |
| `person_id` | fk → Person |  |
| `role` | enum | student | staff | company_hr | tutor |
| `organization_id` | fk → Organization? | si role=company_hr |
| `status` | enum | active | archived | pending |
| `joined_at` | timestamp |  |

> [!note] Nota
> Los cuatro actores (Career Service, RRHH, Tutor, Alumno) se expresan aquí.

Relacionado: [[Entidad - Person]] · [[D-02 Tutor rol global vs por programa]] · [[Modelo de dominio (índice)]]
