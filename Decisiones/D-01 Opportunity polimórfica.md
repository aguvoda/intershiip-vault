---
tags: [decision, resuelto]
---
# D-01 — Opportunity: ¿subtipos o entidad única?

> [!check] RESUELTO (2026-06-09)
> **Opportunity es una entidad única = "una oferta". Sin subtipos.** Se descartan `job / internship / tfg / challenge`. En el sistema hablamos solo de **Opportunity**.

## Consecuencias
- Se elimina el campo `type` de [[Entidad - Opportunity|Opportunity]].
- **Un único flujo de publicación** de ofertas (sin ramificación por tipo).
- Toda oferta puede derivar en un [[Entidad - InternshipRecord|InternshipRecord]] al aceptar una candidatura.
- Desaparecen del modelo los conceptos de challenge y TFG ([[D-07 Challenges y TFG]]) y la entidad Activity.

Relacionado: [[Entidad - Opportunity]] · [[D-07 Challenges y TFG]]
