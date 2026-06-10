---
tags: [arquitectura, core, moc]
---
# Las 5 capas arquitectónicas

El [[Sistema de dos capas]] se implementa con cinco capas:

1. [[Capa - Grafo de entidades]] — quién es quién y cómo se relaciona.
2. [[Capa - Event log]] — cada acción = evento inmutable. Columna vertebral.
3. [[Capa - State machine]] — estados que solo cambian mediante eventos.
4. [[Capa - Policy layer]] — reglas por universidad **como datos, no hardcode**. La clave de la escalabilidad.
5. [[Capa - Agent layer]] — agentes que **asisten sin decidir**.

> [!note] Capas técnicas (cómo) vs capas de producto (qué)
> Estas 5 capas son el **cómo** técnico. El [[Modelo operativo v0.3 (índice)|modelo operativo v0.3]] organiza el **qué** en 8 capas de producto (network activation, relationship, opportunity distribution, student access, practice operations, revenue/reward…). Conviven.

Relacionado: [[ADR-001 - Relational + Event Log]] · [[Modelo de dominio (índice)]] · [[Modelo operativo v0.3 (índice)]]
