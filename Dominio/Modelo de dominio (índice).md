---
tags: [dominio, moc, core]
---
# Modelo de dominio (índice)

> [!check] Decisión (2026-06-09)
> **Fuente de verdad confirmada:** este modelo, con [[Entidad - Opportunity|Opportunity]] como puerta de entrada. El memo queda como contexto histórico. (Resuelve B2.)

Fuente original: `domain-model.jsx`, **simplificado** según decisiones cerradas: Opportunity sin subtipos, sin challenges/TFG, sin Activity; empresa global; MatchThread incorporado.

## Entidades por tipo
- **Root:** [[Entidad - Tenant]]
- **Actores:** [[Entidad - Person]] · [[Entidad - Membership]] · [[Entidad - Organization]] · [[Entidad - StudentProfile]]
- **Contexto:** [[Entidad - AcademicProgram]]
- **Core (flujo):** [[Entidad - Opportunity]] → [[Entidad - Application]] (agrupadas en [[Entidad - MatchThread]]) → [[Entidad - InternshipRecord]]
- **Documentos:** [[Entidad - Agreement]] · [[Entidad - Rubric]] · [[Entidad - Document]]
- **Engagement:** [[Entidad - Conversation y Message]]
- **Governance:** [[Entidad - PolicySet]]
- **Spine:** [[Entidad - Event]]

## Flujo principal
[[Entidad - Opportunity|Opportunity]] (oferta) → recibe [[Entidad - Application|candidaturas]] (agrupadas por candidato en [[Entidad - MatchThread|MatchThread]]) → al aceptar nace el [[Entidad - InternshipRecord|InternshipRecord]] → [[Entidad - Agreement|convenio(s)]] (+ [[Entidad - Rubric|rúbrica]] si curricular).

## Subentidades aún sin esquema
`AuditCase`, `AgreementTemplate`, `RubricTemplate`. (Descartadas: `TutorDelegation` —tutor por programa—, `TFGProposal` y challenges/Activity —fuera de alcance—, `OrganizationTenantLink` —empezamos con perfil global—.)

## Los 4 actores
Career Service ([[Esther (Career Service)]]), RRHH de empresa, Tutor ([[Javier (CETT)]]), Alumno — todos vía [[Entidad - Membership]].

Mapa de relaciones: [[Relaciones del dominio]] · decisiones: [[00 Pendientes y Dudas]]
