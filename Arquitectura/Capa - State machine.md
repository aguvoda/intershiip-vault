---
tags: [arquitectura, capa]
---
# Capa — State machine

Una práctica ([[Entidad - InternshipRecord|InternshipRecord]]) atraviesa estados definidos. **Los estados solo se atraviesan mediante eventos** ([[Capa - Event log]]).

| Estado | Activado por |
|---|---|
| Draft | internship_record.created |
| Proposed | university.validation_requested |
| Validated | university.validated |
| Agreement In Progress | agreement.draft_created |
| Agreement Executed | agreement.fully_executed |
| Active | internship.started |
| Closing | internship.ended |
| Closed | internship.closed |
| On Hold | incident.reported / documentation_missing |
| Cancelled | internship.cancelled (con motivo + traza) |

En el modelo de dominio actual el enum se nombra: `draft → proposed → validated → agreement_in_progress → agreement_executed → active → closing → closed`. Ver [[Entidad - InternshipRecord]].
