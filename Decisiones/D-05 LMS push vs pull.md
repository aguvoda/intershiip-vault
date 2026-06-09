---
tags: [decision, resuelto]
---
# D-05 — LMS: ¿push o pull?

> [!check] RESUELTO PARA MVP (2026-06-09)
> **MVP: export manual / CSV.** Integración automática (LTI 1.3) **post-MVP**. Coherente con N4 (sin integraciones en la primera versión).

## Qué significa (en cristiano)
**LMS** = el sistema de la universidad donde se gestionan cursos y notas (Moodle, Canvas, Blackboard…). Cuando una práctica **curricular** se evalúa ([[Entidad - Rubric|Rubric]]), esa nota tiene que acabar en el cuaderno de notas del LMS.
- **Push (LTI 1.3):** Internshiip.com **empuja** la nota al LMS automáticamente. Más cómodo, pero depende de que cada LMS lo soporte.
- **Pull / CSV:** se **exporta** la nota y la universidad la sube. Más simple, universal.

## Decisión
En el MVP, [[Entidad - Rubric|Rubric]] usa `lms_sync_status=manual` + export. El **adapter layer** y LTI 1.3 llegan cuando se aborden integraciones.

Relacionado: [[Entidad - Rubric]] · [[Tesis 6 - Integration Infrastructure Layer]]
