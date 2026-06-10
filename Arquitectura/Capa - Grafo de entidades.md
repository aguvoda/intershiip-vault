---
tags: [arquitectura, capa]
---
# Capa — Grafo de entidades

Modela quién es quién y cómo se relaciona: universidad, facultad, programa, empresa, estudiante, tutor. Todo conectado en torno a la entidad central.

> [!note] Evolución (v0.3 Relationship Flywheel)
> El centro ya no es ni el expediente ni la oferta: es la **[[Entidad - InstitutionalRelationship|relación institucional]]** universidad↔empresa. La cadena: contacto → [[Entidad - ReferralLead|lead]] → relación → [[Entidad - MasterOpportunity|MasterOpportunity]] → [[Entidad - InstitutionalPosting|InstitutionalPosting]] → [[Entidad - Application|candidatura]] → [[Entidad - PracticeCase|PracticeCase]]. Ver [[Modelo de dominio (índice)]].

Detalle completo: [[Modelo de dominio (índice)]] · [[Relaciones del dominio]]
