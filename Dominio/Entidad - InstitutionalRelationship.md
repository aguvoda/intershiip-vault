---
tags: [dominio, entidad, relationship, core, mvp]
---
# InstitutionalRelationship · _Relación institucional_

> [!info] El activo de red (el moat)
> La relación viva entre un **scope de universidad** y un **scope de empresa**. No es lo mismo que una cuenta (Account) ni que un convenio (FrameworkAgreement). Es la unidad que acumula valor y genera prácticas, resultados y expansión.

| Campo | Nota |
|---|---|
| `id`, `university_id`, `academic_unit_id` | scope universidad |
| `organization_id`, `legal_entity_id`, `site_id` | scope empresa |
| `source`, `owner_user_id` | |
| `status` | discovered → suggested → invited → active → agreement_needed → agreement_signed → opportunities_active · *otros:* dormant / at_risk / strategic |

**Relaciones:** University, AcademicUnit, Organization, LegalEntity, Site, FrameworkAgreement, [[Entidad - MasterOpportunity]], [[Entidad - PracticeCase]]. **MVP:** Sí.

Relacionado: [[Relationship flywheel]] · [[Moat (ventaja competitiva)]] · [[Tesis 1 - Relationship Expansion Engine]]
