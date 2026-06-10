---
tags: [arquitectura, capa, core]
---
# Capa — Event log

Cada acción relevante genera un **evento inmutable**. Es la columna vertebral del sistema: da trazabilidad, auditoría, analítica y aprendizaje progresivo. Es la base del [[Moat (ventaja competitiva)|moat]] (≈ Foundry de Palantir).

En v0.3 la entidad concreta es [[Entidad - AttributionEvent|AttributionEvent]] (append-only): sirve a crecimiento, billing, rewards, compliance y auditoría a la vez.

## Estructura del evento
| Campo | Ejemplo |
|---|---|
| entity_type, entity_id | practice_case / specific_agreement / referral_lead |
| event_type | agreement.fully_signed / posting.published / lead.converted_paid |
| source_actor_type, source_user_id | university_staff / company_admin / agent / system |
| metadata (JSON), created_at | |

> [!note] Regla de oro
> No hay escrituras directas de estado. El estado cambia **solo mediante eventos** ([[Capa - State machine]]). Append-only desde el MVP: registra quién subió un contacto, quién aprobó una invitación, cuándo una MasterOpportunity pasó a InstitutionalPosting, cuándo un SpecificAgreement quedó fully_signed y qué SuccessFeeEvent generó.

Ver entidad [[Entidad - AttributionEvent]] · decisión [[ADR-001 - Relational + Event Log]].
