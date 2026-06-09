---
tags: [arquitectura, stack, resuelto]
---
# Stack técnico

> [!check] RESUELTO (2026-06-09)
> Stack definido por el [[Agu (CTO)|CTO]].

| Capa | Tecnología |
|---|---|
| **API / Backend** | **.NET 10** |
| **Frontend web** | **Next.js + React** (deploy en **Vercel**) — superficie desktop de universidad y empresa ([[Tesis 4 - Channel-Specific Experience]]) |
| **App móvil** | **Flutter** — superficie del alumno |
| **Base de datos** | **PostgreSQL** — estado relacional + tabla `event_log` append-only ([[ADR-001 - Relational + Event Log]]) |
| **Infraestructura** | **Azure Cloud** — multi-tenant, GDPR desde el día uno |

> [!note] Cambio respecto al briefing
> El briefing proponía Node/Python(FastAPI); la decisión final del CTO es **.NET 10**. El resto de principios (event-driven, Postgres + event log, multi-tenant, GDPR) se mantienen.

## Pendiente
- [ ] **Agent layer**: motor de IA para parseo/coordinación (el briefing proponía Claude API). Confirmar proveedor. Ver [[Capa - Agent layer]].
- [ ] Motor documental + proveedor de firma (Signaturit/DocuSign).

Relacionado: [[ADR-001 - Relational + Event Log]] · [[Agu (CTO)]]
