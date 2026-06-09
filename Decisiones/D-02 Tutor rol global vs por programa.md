---
tags: [decision, resuelto]
---
# D-02 — Tutor: ¿rol global o por programa?

> [!check] RESUELTO (2026-06-09)
> El **tutor se asigna por programa** ([[Entidad - AcademicProgram|AcademicProgram]]), no como rol global con delegación.

## Consecuencias
- Cada [[Entidad - AcademicProgram|programa]] tiene su(s) tutor(es) asignado(s); el [[Entidad - InternshipRecord|InternshipRecord]] hereda el tutor del programa del alumno.
- **Se elimina** la necesidad de `TutorDelegation` (era para el modelo de "tutor global que delega"). Ya no aplica.

> [!note] Modelado sugerido
> Mapeo `AcademicProgram → tutor(es)` (vía [[Entidad - Membership|Membership]] con `role=tutor` ligada al programa). Pendiente de detalle fino en el esquema.

Relacionado: [[Entidad - Membership]] · [[Entidad - AcademicProgram]]
