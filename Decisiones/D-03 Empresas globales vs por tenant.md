---
tags: [decision, resuelto]
---
# D-03 — Empresas: ¿globales o por tenant?

> [!check] RESUELTO (2026-06-09)
> **Empezamos con perfil GLOBAL.** Una empresa = un perfil único compartido entre centros. La data sensible (ofertas, candidaturas, conversaciones) ya queda aislada por `tenant_id` en sus propias entidades.

## Consecuencias
- [[Entidad - Organization]] global (perfil único, refuerza el efecto red de [[Tesis 1 - Relationship Expansion Engine]]).
- `OrganizationTenantLink` **no se necesita** en la primera versión (futuro, si hace falta verificación por centro).

Relacionado: [[Entidad - Organization]] · [[Entidad - Tenant]]
