---
tags: [dominio, entidad, practice-operations, core, mvp]
---
# SpecificAgreement · _Convenio específico_

Convenio específico para un alumno, empresa, universidad y [[Entidad - PracticeCase|PracticeCase]]. Sustituye a `Agreement` v0.2. **Su firma completa dispara la monetización.**

| Campo | Nota |
|---|---|
| `id`, `practice_case_id`, `version`, `document_id` | |
| `status` | draft → pending_data → pending_review → pending_signature → fully_signed / cancelled |
| `generated_at`, `fully_signed_at` | |

> [!important] El [[Entidad - SuccessFeeEvent|SuccessFeeEvent]] se dispara en `fully_signed` (más auditable que "candidato seleccionado", más cercano al valor real que "oferta publicada").

> [!note] FrameworkAgreement (convenio marco)
> El convenio **marco** (cobertura por centro/programa/tipo) es distinto del específico. Vive a nivel [[Entidad - InstitutionalRelationship|relación]]/[[Entidad - PracticePolicy|política]]; si falta, el `DistributionTarget` queda en `needs_agreement`. Motor de coverage completo → fase 2 ([[Entidad - Avanzadas (fase 2)]]).

**Relaciones:** [[Entidad - PracticeCase]] · [[Entidad - SignatureRequest]] · [[Entidad - SuccessFeeEvent]]. **MVP:** Sí.

Relacionado: [[Capa - State machine]] · [[Modelo de monetización]]
