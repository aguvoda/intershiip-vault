---
tags: [decision, resuelto]
---
# D-03 — Empresas: ¿globales o por tenant?

> [!check] RESUELTO (2026-06-09)
> **Empezamos con perfil GLOBAL.** Una empresa ([[Entidad - Organization|Organization]]) = un perfil único compartido entre centros. La data sensible (ofertas, candidaturas) ya queda aislada por scope de universidad/centro en sus propias entidades.

## Consecuencias
- [[Entidad - Organization]] global (perfil único, refuerza el efecto red de [[Tesis 1 - Relationship Expansion Engine]]).
- `OrganizationTenantLink` **no se necesita** en la primera versión (futuro, si hace falta verificación por centro).

Relacionado: [[Entidad - Organization]] · [[Entidad - University]] · [[Cuentas, roles y trust levels]]
