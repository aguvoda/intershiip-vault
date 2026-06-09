---
tags: [dominio, entidad, core]
---
# InternshipRecord · _Expediente_

> Una práctica confirmada. El antiguo centro.

Nace cuando una [[Entidad - Application|Application]] para una [[Entidad - Opportunity|Opportunity]] de tipo internship es aceptada. Gestiona el ciclo post-match: convenio, tutor, rúbrica, cierre. **Única entidad con [[Capa - State machine|state machine]] propia.**

## Campos
| Campo | Tipo | Nota |
|---|---|---|
| `id` | uuid | IR-2026-0347 |
| `tenant_id` | fk → Tenant |  |
| `application_id` | fk → Application |  |
| `opportunity_id` | fk → Opportunity | denorm |
| `student_profile_id` | fk → StudentProfile | denorm |
| `organization_id` | fk → Organization | denorm |
| `tutor_membership_id` | fk → Membership? | solo si curricular |
| `modality` | enum | curricular | extracurricular | mixed |
| `total_hours` | int |  |
| `curricular_hours` | int | subset de total |
| `start_date` | date |  |
| `end_date` | date |  |
| `state` | enum | draft | proposed | validated | agreement_in_progress | agreement_executed | active | closing | closed |
| `policy_snapshot_id` | fk → PolicySet | política vigente al crear |

> [!note] Nota
> Conserva el state machine del memo. Pero ya no entra por la puerta — entra un Opportunity.

Relacionado: [[Capa - State machine]] · [[Entidad - Agreement]] · [[D-06 Convenio curricular + extracurricular]] · [[Modelo de dominio (índice)]]
