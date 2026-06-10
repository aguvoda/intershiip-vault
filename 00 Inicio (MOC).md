---
tags: [moc, inicio]
---
# 🗺️ Internshiip.com — Mapa del vault

> [!info] Qué es este vault
> Conocimiento estructurado del proyecto **Internshiip.com**, extraído del Claude Design de Xavi (memos, briefing CTO, tesis, sistema de diseño y modelo de dominio). Notas atómicas enlazadas. Lo **pendiente de definir** está marcado y centralizado en [[00 Pendientes y Dudas]].

## En una frase
Infraestructura de **coordinación institucional** para prácticas universitarias, vendida como **[[Modelo RaaS]]**, con lógica **[[Modelo de referencia - Palantir|Palantir]]**. La apuesta: las prácticas no son un problema de matching sino de coordinación.

## Negocio
- [[El problema]] · [[La hipótesis]] · [[Modelo RaaS]] · [[Modelo de referencia - Palantir]]
- [[Panorama competitivo]] · [[Mercado (TAM SAM SOM)]] · [[Moat (ventaja competitiva)]]
- [[Pricing]] · [[Roadmap 12 meses]] · [[Estrategia de entrada (GTM)]] · [[Equipo]]

## Lanzamiento (Founding Partner)
- [[Founding Partner Program]] · [[Posicionamiento y mensaje]] · [[Guía de tono y copy]] · [[Cliente ideal (ICP)]]
- [[Métricas del caso de éxito]] · [[Materiales de venta]] · [[Plan de lanzamiento 30 días]]

## Producto — Modelo operativo v0.3
- [[Modelo operativo v0.3 (índice)]] · [[Relationship flywheel]] · [[Modelo de monetización]] · [[Distribución MasterOpportunity vs InstitutionalPosting]]
- [[Cuentas, roles y trust levels]] · [[Workflows canónicos]] · [[MVP v0.3]] · [[Cumplimiento y datos (compliance)]]

### 6 tesis
[[Tesis 1 - Relationship Expansion Engine]] · [[Tesis 2 - Institutional Relationship Discovery]] · [[Tesis 3 - Diseñar desde la universidad más compleja]] · [[Tesis 4 - Channel-Specific Experience]] · [[Tesis 5 - Voice-First Student Experience]] · [[Tesis 6 - Integration Infrastructure Layer]]

## Arquitectura
- [[Sistema de dos capas]] · [[Las 5 capas]] · [[ADR-001 - Relational + Event Log]]
- Capas: [[Capa - Grafo de entidades]] · [[Capa - Event log]] · [[Capa - State machine]] · [[Capa - Policy layer]] · [[Capa - Agent layer]]
- Agentes: [[Agente - Intake & Structuring]] · [[Agente - Agreement Coordinator]] · [[Agente - Compliance & Audit]]
- [[Stack técnico]]

## Dominio (v0.3, 8 capas)
[[Modelo de dominio (índice)]] · [[Relaciones del dominio]] — entidades core: [[Entidad - InstitutionalRelationship|InstitutionalRelationship]] · [[Entidad - MasterOpportunity|MasterOpportunity]] · [[Entidad - InstitutionalPosting|InstitutionalPosting]] · [[Entidad - PracticeCase|PracticeCase]] · [[Entidad - SpecificAgreement|SpecificAgreement]] · [[Entidad - SuccessFeeEvent|SuccessFeeEvent]] · [[Entidad - ReferralLead|ReferralLead]]

## Decisiones
[[D-02 Tutor rol global vs por programa]] · [[D-03 Empresas globales vs por tenant]] · [[D-05 LMS push vs pull]] · [[D-06 Convenio curricular + extracurricular]] · [[D-07 Challenges y TFG]] · [[D-08 Chat quién inicia con quién]] · [[D-09 Formación dual]]
> _D-01 (Opportunity única) y D-04 (MatchThread) eliminadas: superadas por v0.3._

## Diseño
[[Sistema de diseño]] · [[Design tokens]] · [[Logo e isotipo]] · [[Componentes UI]] · [[Manifiesto visual]]

## Personas y discovery
[[Xavi (CEO)]] · [[Agu (CTO)]] · [[Javier (CETT)]] · [[Esther (Career Service)]] · [[CETT (cliente piloto)]] · [[Guía de entrevista a decisores]]

## Fuentes
[[Índice de archivos originales]]
