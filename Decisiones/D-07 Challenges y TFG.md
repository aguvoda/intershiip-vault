---
tags: [decision, resuelto]
---
# D-07 — Challenges y TFG

> [!check] RESUELTO (2026-06-09)
> **Fuera del modelo.** El MVP cubre únicamente [[Entidad - Opportunity|Opportunity]] = una oferta. **Challenges y TFG se eliminan** del modelo (no son subtipos de oferta), y con ellos la entidad **Activity**.

## Consecuencias
- Sin `type=challenge` ni `type=tfg_tfm`.
- Entidad **Activity eliminada** (existía para alojar challenges/eventos).
- `TFGProposal` descartado.
- Si en el futuro se quieren retos/eventos/TFG, se rediseñan como módulo aparte.

Relacionado: [[Entidad - Opportunity]] · [[D-01 Opportunity polimórfica]]
