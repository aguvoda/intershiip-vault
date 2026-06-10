---
tags: [decision, resuelto]
---
# D-07 — Challenges y TFG

> [!check] RESUELTO (2026-06-09)
> **Fuera del modelo.** El MVP cubre únicamente prácticas ([[Entidad - MasterOpportunity|MasterOpportunity]] → [[Entidad - InstitutionalPosting|InstitutionalPosting]]). **Challenges y TFG se eliminan** del modelo, y con ellos la entidad **Activity**. v0.3 lo confirma (excluye eventos/retos/TFG/TFM del MVP).

## Consecuencias
- Sin `type=challenge` ni `type=tfg_tfm`.
- Entidad **Activity eliminada** (existía para alojar challenges/eventos).
- `TFGProposal` descartado.
- Si en el futuro se quieren retos/eventos/TFG, se rediseñan como módulo aparte.

Relacionado: [[Entidad - MasterOpportunity]] · [[MVP v0.3]]
