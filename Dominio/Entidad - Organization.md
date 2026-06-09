---
tags: [dominio, entidad, actor]
---
# Organization · _Empresa colaboradora_

> [!check] Decisión D-03 (2026-06-09)
> **Empezamos con un perfil GLOBAL** (único, compartido entre centros). La data sensible (ofertas, candidaturas, conversaciones) ya queda aislada por `tenant_id` en sus propias entidades. Ver [[D-03 Empresas globales vs por tenant]].

Una empresa con perfil rico (employer branding): descripción, sectores, fotos, vídeos, testimonios, cultura. Perfil único; su presencia en cada centro se da a través de las ofertas que publica allí.

## Campos
| Campo | Tipo | Nota |
|---|---|---|
| `id` | uuid | |
| `legal_name` | string | Acme Hotels SL |
| `display_name` | string | Acme Hotels |
| `vat_id` | string | CIF/NIF |
| `sectors` | string[] | hotelería, gastronomía… |
| `size` | enum | startup \| sme \| large |
| `logo_url` | string | |
| `cover_url` | string? | |
| `description` | markdown | pitch |
| `culture_media` | Media[] | fotos/vídeos |
| `verified` | boolean | validada por Career Service |

> [!note] Futuro (no MVP)
> Si más adelante hiciera falta verificación/relación **por centro**, se añadiría un `OrganizationTenantLink`. No se necesita en la primera versión.

Relacionado: [[Entidad - Opportunity]] · [[Tesis 1 - Relationship Expansion Engine]] · [[Modelo de dominio (índice)]]
