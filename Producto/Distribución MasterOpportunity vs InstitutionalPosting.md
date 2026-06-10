---
tags: [producto, distribucion, core]
---
# Distribución: MasterOpportunity vs InstitutionalPosting

Reconcilia dos verdades opuestas: la empresa quiere **distribución amplia**; la universidad quiere **contenido institucional controlado**.

> [!note] Regla de producto
> La empresa crea **una** [[Entidad - MasterOpportunity|MasterOpportunity]]. Cada universidad/centro recibe su propia [[Entidad - InstitutionalPosting|InstitutionalPosting]]. El alumno ve la publicación institucional, no un listado de marketplace genérico. **Eso no es un job board: es distribución institucional controlada.**

## Estados del DistributionTarget
| Estado | Lenguaje a la empresa | Acción interna |
|---|---|---|
| `can_publish_now` | Listo para revisión | crear InstitutionalPosting |
| `needs_review` | Esperando revisión institución | avisar coordinador |
| `needs_agreement` | Convenio requerido antes de publicar | crear tarea de convenio |
| `needs_activation` | Solicitar activación | crear [[Entidad - ReferralLead]] / [[Entidad - CompanyInterest]] |
| `contact_needed` | Falta contacto | [[Entidad - InternalAlert]] + research |
| `rejected` | No aceptado | registrar motivo |

## Modos de visibilidad
- `private_institutional` — alumnos de una institución/unidad. **Default** para prácticas institucionales.
- `shared_selected` — varias publicaciones, cada una controlada por su institución. Multi-universidad sin sensación de marketplace.
- `public_preview` — visitantes ven info limitada (SEO, captación demanda). Sin apply formal directo.
- `public_open` — evitar en MVP.

## UX
- Empresa: "**Solicitar distribución**", no "Publicar en todas partes". Grupos: activas / conocidas-limitadas / sugeridas / contacto-necesario. Dashboard de estado por institución. Seleccionar target ≠ publicación garantizada.
- Universidad: ve el posting como enviado a **su** tablón; personaliza programas, requisitos, texto y reglas; ve estado de relación/convenio/origen.

Relacionado: [[Modelo de dominio (índice)]] · [[Relaciones del dominio]] · [[Workflows canónicos]]
