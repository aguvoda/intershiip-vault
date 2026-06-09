---
tags: [arquitectura, capa, agentes]
---
# Capa — Agent layer

Agentes que **asisten sin decidir**. Convierten inputs no estructurados en datos, coordinan convenios y detectan incumplimientos. El humano siempre tiene la última palabra ([[Modelo de referencia - Palantir|human-in-the-loop irrenunciable]]).

## Los tres agentes
- [[Agente - Intake & Structuring]]
- [[Agente - Agreement Coordinator]]
- [[Agente - Compliance & Audit]]

> [!warning] Límites estrictos (en lanzamiento)
> - NO cambia estados sin confirmación humana.
> - NO firma ni ejecuta acciones legales.
> - Solo propone, basándose en: [[Capa - Policy layer|policy]] + [[Capa - Event log|event log]] + datos del registro.

Implementación propuesta: Claude API (Anthropic). Ver [[Stack técnico]].
