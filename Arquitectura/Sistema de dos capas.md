---
tags: [arquitectura, core]
---
# Sistema de dos capas

> [!note] Principio de diseño
> Internshiip.com **no se diseña como una app con pantallas**. Se diseña como un sistema de dos capas.

- **System of Record** — una práctica existe "de verdad" solo cuando está **registrada, versionada y trazada**. *Si no está en el [[Capa - Event log|event log]], no ocurrió.*
- **System of Action** — orquesta tareas, aprobaciones, documentos y comunicaciones. **No sustituye a las personas**: les da visibilidad y les quita fricción.

Se concreta en [[Las 5 capas]]. Decisión fundacional en [[ADR-001 - Relational + Event Log]].
Origen conceptual: [[La hipótesis]].
