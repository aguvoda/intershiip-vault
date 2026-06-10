---
tags: [arquitectura, agentes]
---
# Agente — Agreement Coordinator

**Activador:** estado `agreement_draft` del [[Entidad - PracticeCase|PracticeCase]].
**Función:** genera borradores de [[Entidad - SpecificAgreement|convenio específico]] desde plantillas, detecta inconsistencias (fechas, NIF, programa) e impulsa la secuencia de firma con recordatorios.

> [!warning] No firma
> Solo coordina y prepara. La firma y la ejecución legal requieren actor humano ([[Capa - Agent layer]]).

Relacionado: [[D-06 Convenio curricular + extracurricular]].
