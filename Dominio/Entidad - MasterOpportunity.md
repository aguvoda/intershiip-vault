---
tags: [dominio, entidad, opportunity-distribution, core, mvp]
---
# MasterOpportunity · _Oferta madre_

Oferta/intención creada por la **empresa una vez**, que puede distribuirse a una o varias instituciones. Junto con [[Entidad - InstitutionalPosting|InstitutionalPosting]] sustituye al `Opportunity` único v0.2.

| Campo | Nota |
|---|---|
| `id`, `organization_id`, `legal_entity_id`, `site_id` | |
| `title`, `description`, `location`, `modality`, `hours`, `dates` | `modality`: curricular \| extracurricular \| mixed |
| `status` | draft → ready_for_distribution → distributed → closed · *otros:* cancelled / archived |

> [!note] La empresa crea **una vez**; cada institución recibe su propia [[Entidad - InstitutionalPosting|publicación]]. Ver [[Distribución MasterOpportunity vs InstitutionalPosting]].

**Relaciones:** [[Entidad - Organization]] · [[Entidad - DistributionTarget]] · [[Entidad - InstitutionalPosting]]. **MVP:** Sí.

Relacionado: [[Distribución MasterOpportunity vs InstitutionalPosting]] · [[D-06 Convenio curricular + extracurricular]]
