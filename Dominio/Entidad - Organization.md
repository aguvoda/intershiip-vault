---
tags: [dominio, entidad, company-structure, mvp]
---
# Organization · _Empresa / grupo_

Grupo comercial o marca empleadora (Hotusa, Grupotel, Meliá). Perfil **global** (decisión [[D-03 Empresas globales vs por tenant|D-03]]); su presencia en cada centro se da vía las publicaciones que distribuye.

| Campo | Nota |
|---|---|
| `id`, `name`, `domain`, `industry` | |
| `account_status` | invited \| active \| suspended |
| perfil rico (employer branding) | descripción, sectores, cultura, media — para Employer Presence ([[Pricing]]) |

> [!warning] Una empresa **≠ un CIF**. Las responsabilidades legales y firmas viven en [[Entidad - LegalEntity]] / [[Entidad - Site]].

**Dedupe:** tax_id, domain, nombre normalizado → revisión manual de conflictos.

**Relaciones:** [[Entidad - LegalEntity]] · [[Entidad - Site]] · [[Entidad - MasterOpportunity]] · [[Entidad - ReferralLead]]. **MVP:** Sí.

Relacionado: [[Tesis 1 - Relationship Expansion Engine]] · [[Modelo de dominio (índice)]]
