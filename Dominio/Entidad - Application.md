---
tags: [dominio, entidad, core]
---
# Application · _Candidatura_

> Un alumno se apunta o es sugerido a una oferta.

Relación alumno ↔ [[Entidad - Opportunity|oferta]]. Origen: inbound (el alumno se apunta), outbound (Career Service lo sugiere tras casación) o matching asistido (el sistema propone). Guarda el trayecto: aplicado → entrevista → aceptado → confirmado. Se agrupa en un [[Entidad - MatchThread|MatchThread]] por candidato.

## Campos
| Campo | Tipo | Nota |
|---|---|---|
| `id` | uuid | |
| `opportunity_id` | fk → Opportunity | |
| `student_profile_id` | fk → StudentProfile | |
| `match_thread_id` | fk → MatchThread? | agrupa las candidaturas del alumno |
| `source` | enum | inbound \| suggested_by_staff \| matched_by_agent |
| `status` | enum | applied \| viewed \| interview \| offered \| accepted \| declined \| withdrawn |
| `cover_note` | markdown? | |
| `match_score` | float? | 0–1 si vino del agent |
| `match_rationale` | markdown? | por qué el agent lo sugirió |
| `created_at` | timestamp | |

> [!note] Nota
> Al llegar a `status=accepted`, se genera un [[Entidad - InternshipRecord|InternshipRecord]].

Relacionado: [[Entidad - MatchThread]] · [[Entidad - Opportunity]] · [[Entidad - InternshipRecord]] · [[Modelo de dominio (índice)]]
