---
tags: [decision, resuelto]
---
# D-08 — Chat: ¿quién inicia con quién?

> [!check] RESUELTO (2026-06-09)
> El chat lo inicia **la empresa o la universidad (Career Service). El alumno NUNCA inicia** una conversación.

## Reglas
- **Empresa → (alumno / Career Service):** puede iniciar.
- **Universidad / Career Service → (alumno / empresa):** puede iniciar.
- **Alumno:** **no puede iniciar**; solo **responde** a conversaciones abiertas por empresa o universidad.

> [!note] Implicación de modelado
> En [[Entidad - Conversation y Message|Conversation]], al crear el hilo se valida que el iniciador tenga `role` ∈ {company_hr, staff/tutor}. El alumno aparece como participante pero no como creador. Reduce spam y protege al alumno.

Relacionado: [[Entidad - Conversation y Message]] · [[Capa - Policy layer]]
