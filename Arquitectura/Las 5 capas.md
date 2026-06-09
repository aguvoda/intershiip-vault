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

Relacionado: [[ADR-001 - Relational + Event Log]] · [[Modelo de dominio (índice)]]
