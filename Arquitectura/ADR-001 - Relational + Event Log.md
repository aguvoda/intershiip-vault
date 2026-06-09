---
tags: [arquitectura, adr, core]
---
# ADR-001 — Relational System of Record + Event Log obligatorio

> [!note] Decisión
> Modelo **híbrido**: el estado actual se guarda en **tablas relacionales**; **cada cambio de estado genera un evento** en una tabla `event_log` de solo anexado.

## Por qué no las alternativas
- **Event Sourcing puro** → demasiada complejidad para un equipo pequeño en fase temprana.
- **CRUD puro** → sin capacidad de auditoría.

El híbrido da **velocidad de MVP + fiabilidad de grado institucional**, base para analítica futura y compatibilidad con [[Capa - Agent layer|agentes de IA]].

> [!tip] Es la piedra de toque del CTO
> El briefing pide que el CTO, al leer este ADR, "tenga algo que decir, no que asentir". Ver [[Agu (CTO)]].

Relacionado: [[Capa - Event log]] · [[Capa - State machine]] · [[Stack técnico]]
