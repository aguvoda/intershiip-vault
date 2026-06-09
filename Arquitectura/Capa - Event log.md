---
tags: [arquitectura, capa, core]
---
# Capa — Event log

Cada acción relevante genera un **evento inmutable**. Es la columna vertebral del sistema: da trazabilidad, auditoría, analítica y aprendizaje progresivo. Es la base del [[Moat (ventaja competitiva)|moat]] (≈ Foundry de Palantir).

## Estructura del evento (del memo)
| Campo | Tipo | Ejemplo |
|---|---|---|
| event_id | UUID | evt_a1b2c3… |
| timestamp | ISO8601 | 2026-04-14T10:32:00Z |
| actor_type | Enum | university_staff / student / agent / system |
| entity_type | Enum | internship_record / agreement / evaluation |
| event_type | String | agreement.signed_by_company |
| payload | JSON | { party: 'company', signed_at: '…' } |
| source | Enum | manual / email_ingest / integration / agent |

> [!note] Regla de oro
> No hay escrituras directas de estado. El estado cambia **solo mediante eventos** ([[Capa - State machine]]).

Ver entidad [[Entidad - Event]] · decisión [[ADR-001 - Relational + Event Log]].
