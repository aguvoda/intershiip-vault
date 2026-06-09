---
tags: [dominio, relaciones]
---
# Relaciones del dominio

| Origen | Cardinalidad | Destino | Condición |
|---|---|---|---|
| [[Entidad - Tenant\|Tenant]] | 1..n | Membership | |
| Tenant | 1..n | Opportunity | |
| Tenant | 1..n | AcademicProgram | |
| Tenant | 1..n | PolicySet | |
| [[Entidad - Person\|Person]] | 1..n | Membership | |
| [[Entidad - Membership\|Membership]] | 0..1 | StudentProfile | si role=student |
| Membership | 0..1 | Organization | si role=company_hr |
| [[Entidad - Organization\|Organization]] | 1..n | Opportunity | |
| [[Entidad - Opportunity\|Opportunity]] | 1..n | Application | |
| [[Entidad - StudentProfile\|StudentProfile]] | 1..n | Application | |
| StudentProfile | 1..n | MatchThread | trayecto de candidaturas |
| [[Entidad - MatchThread\|MatchThread]] | 1..n | Application | agrupa |
| [[Entidad - Application\|Application]] | 0..1 | InternshipRecord | al aceptar (accepted) |
| [[Entidad - InternshipRecord\|InternshipRecord]] | 1..n | Agreement | versionados |
| InternshipRecord | 0..1 | Rubric | si curricular |
| InternshipRecord | 0..1 | Membership | tutor (por programa), si curricular |
| [[Entidad - Conversation y Message\|Conversation]] | n..n | Membership | participantes |
| Conversation | 0..1 | Opportunity/Application/InternshipRecord | contexto |

**Flujo:** Opportunity → Application (→ MatchThread por candidato) → (si accepted) → InternshipRecord → Agreement(s) (+ Rubric si curricular).

Relacionado: [[Modelo de dominio (índice)]]
