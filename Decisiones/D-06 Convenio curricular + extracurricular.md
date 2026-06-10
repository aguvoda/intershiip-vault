---
tags: [decision, resuelto]
---
# D-06 — Convenio curricular + extracurricular

> [!check] RESUELTO (2026-06-09)
> **Sí, soportar `modality=mixed`.** Una oferta/práctica puede ser curricular, extracurricular o **mixta**, en un solo convenio.

## Curricular vs extracurricular
| | **Curricular** | **Extracurricular** |
|---|---|---|
| Qué es | Parte del plan de estudios | Voluntaria, fuera del plan |
| Créditos | Cuenta créditos | No cuenta |
| Tutor / evaluación | Requiere tutor + [[Entidad - Avanzadas (fase 2)|evaluación]] | No requiere |
| Horas | **Mínimo** (ej. 250h) | **Máximo** (ej. 900h) |

## Consecuencias
- `modality = curricular | extracurricular | mixed` en [[Entidad - MasterOpportunity|MasterOpportunity]] y [[Entidad - PracticeCase|PracticeCase]].
- En `mixed`: `curricular_hours` declara la parte curricular; el resto es extracurricular. La plantilla de [[Entidad - SpecificAgreement|convenio]] lo resuelve con cláusulas condicionales.

Relacionado: [[Entidad - PracticeCase]] · [[Entidad - SpecificAgreement]] · [[Entidad - PracticePolicy]]
