---
tags: [dominio, entidad, avanzadas, fase-2]
---
# Entidades avanzadas (fase 2)

Entidades del modelo v0.3 marcadas como **Later / partial**. No bloquean el MVP; se definen cuando el loop básico está probado. Agrupadas aquí para no crear notas vacías ([[Modelo de dominio (índice)]]).

| Entidad | Capa | Para qué |
|---|---|---|
| **HoursRecord** | Practice ops | Registro de horas pactadas/realizadas |
| **Incident** | Practice ops | Incidencias durante la práctica |
| **Addendum** | Practice ops | Anexos/modificaciones del convenio |
| **Evaluation** | Practice ops | Evaluación académica (sustituye `Rubric` v0.2) |
| **Certificate** | Practice ops | Certificado de prácticas |
| **EmploymentOutcome** | Practice ops | Si el alumno acabó contratado (dato de empleabilidad) |
| **RelationshipHealthScore** | Relationship | Score de calidad/confianza/actividad de una [[Entidad - InstitutionalRelationship\|relación]] |
| **FrameworkAgreement** | Company/Relationship | Convenio **marco** (cobertura); ver [[Entidad - SpecificAgreement]] |

> [!note] El reporting de empleabilidad ([[Métricas del caso de éxito]]) se alimenta sobre todo de Evaluation, EmploymentOutcome y Certificate. Construir cuando el flujo firma→fee sea fiable.

Roadmap: [[MVP v0.3]] · [[Roadmap 12 meses]]
