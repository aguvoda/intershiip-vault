---
tags: [dominio, entidad, revenue-reward, core, mvp]
---
# SuccessFeeEvent · _Evento de fee por práctica_

Evento de facturación creado cuando una práctica firmada cumple el disparador. Es la **"práctica activada"** del [[Pricing]] (39 € oficial / 29 € early / 19 € ultra early).

| Campo | Nota |
|---|---|
| `id`, `practice_case_id`, `organization_id`, `amount`, `trigger` | |
| `status` | pending → invoice_ready → invoiced → paid · *otros:* credited / disputed / cancelled |

> [!important] Aunque las facturas sean manuales, **este evento debe existir** (atribución de billing nativa al producto). Disparador: [[Entidad - SpecificAgreement]] `fully_signed`.
> **Cancelación:** crédito/refund si se cancela antes de empezar por causa alumno/universidad; sin refund automático si la empresa cancela tras firma.

**Relaciones:** [[Entidad - PracticeCase]] · [[Entidad - SpecificAgreement]] · [[Entidad - Organization]] · [[Entidad - University]]. **MVP:** Sí.

Relacionado: [[Modelo de monetización]] · [[Pricing]]
