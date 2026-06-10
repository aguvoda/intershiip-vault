---
tags: [dominio, entidad, opportunity-distribution, mvp]
---
# DistributionTarget · _Objetivo de distribución_

Una institución o scope académico objetivo de una [[Entidad - MasterOpportunity|MasterOpportunity]].

| Campo | Nota |
|---|---|
| `id`, `master_opportunity_id`, `target_university_id`, `target_academic_unit_id` | |
| `target_status` | can_publish_now \| needs_review \| needs_agreement \| needs_activation \| contact_needed \| rejected |
| `status` | selected → can_publish_now → institutional_posting_created |

> [!warning] Distinción clave
> **Seleccionar un target no garantiza publicación.** Según `target_status`: `can_publish_now` → crear [[Entidad - InstitutionalPosting]]; `needs_activation` → [[Entidad - ReferralLead]]/[[Entidad - CompanyInterest]]; `contact_needed` → [[Entidad - InternalAlert]].

**Relaciones:** [[Entidad - MasterOpportunity]] · [[Entidad - SuggestedInstitution]] · [[Entidad - InstitutionalPosting]] · [[Entidad - CompanyInterest]]. **MVP:** Sí.

Relacionado: [[Distribución MasterOpportunity vs InstitutionalPosting]]
