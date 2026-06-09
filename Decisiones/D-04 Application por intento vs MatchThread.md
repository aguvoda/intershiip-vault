---
tags: [decision, resuelto]
---
# D-04 — Application por intento + MatchThread

> [!check] RESUELTO (2026-06-09)
> **Sí a MatchThread.** [[Entidad - Application|Application]] sigue siendo atómica (un intento a una oferta) y se incorpora [[Entidad - MatchThread|MatchThread]] para **ver todas las candidaturas de un candidato** (todas las ofertas a las que aplicó) en un solo sitio.

## Consecuencias
- Nueva entidad [[Entidad - MatchThread]] (esquema definido).
- `Application.match_thread_id` (opcional) enlaza cada candidatura a su trayecto.
- Vista pensada para Career Service / prospección dirigida.

Relacionado: [[Entidad - MatchThread]] · [[Entidad - Application]]
