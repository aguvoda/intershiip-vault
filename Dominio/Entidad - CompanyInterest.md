---
tags: [dominio, entidad, opportunity-distribution, mvp]
---
# CompanyInterest · _Interés de empresa_

Una empresa expresa interés en publicar con una institución **no activa o no contactable**. Es una **señal de venta caliente**, no una publicación automática.

| Campo | Nota |
|---|---|
| `id`, `status` | interest_recorded → contact_needed → contact_research_pending → ready_to_outreach → outreach_sent → converted_to_referral_lead |

**Relaciones:** [[Entidad - MasterOpportunity]] · [[Entidad - SuggestedInstitution]] · [[Entidad - ReferralLead]] · [[Entidad - InternalAlert]]. **MVP:** Sí.

Relacionado: [[Relationship flywheel]] · [[Distribución MasterOpportunity vs InstitutionalPosting]]
