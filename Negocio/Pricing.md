---
tags: [negocio, pricing, core]
---
# Pricing

> [!check] Fuente definitiva (2026-06-10)
> Modelo de **Product & Pricing Strategy v0.1**. Sustituye al catálogo SaaS viejo y a los números del Launch (School 18k/Inst 48k quedan **descartados**). Reconcilia la tensión RaaS↔catálogo de [[Modelo RaaS]].

## Qué cobramos realmente
No cobramos por usuarios, pantallas ni publicaciones. Cobramos por **absorber dolor operativo** y convertir una relación informal universidad-empresa en un flujo trazable. Dos lógicas:
- **Universidad financia el core** → planes anuales por volumen, centros e integraciones.
- **Empresa entra sin fricción y paga por relación** → acceso operativo incluido + planes de presencia/engagement/network + **fee por práctica activada** ([[Entidad - SuccessFeeEvent|SuccessFeeEvent]]).

> [!note] Principios no negociables
> Precio ligado al *pain* · no parecer job board · no parecer comisión (el fee se llama "práctica activada") · mensual ~20% más caro · early adopter **no eterno** · anchoring premium (13k → 150k+).

## Universidad — Internshiip for Institutions
| Plan | Anual | Equiv. mensual | Pago mensual | Cliente |
|---|---|---|---|---|
| **School** | 13.000 € | 1.083 € | 1.300 € | Escuela / centro / institución pequeña |
| **Institution** | 36.000 € | 3.000 € | 3.600 € | Universidad privada / grupo / multi-centro medio |
| **University Pro** | 72.000 € | 6.000 € | 7.200 € | Universidad grande, varios centros/programas |
| **Enterprise** | desde 150.000 € | desde 12.500 € | desde 15.000 € | Alta complejidad, integraciones, multi-campus |

**Incluye (acumulativo):**
- **School** — importación de empresas, tablón institucional, validación de ofertas, [[Entidad - PracticeCase|PracticeCase]] básico, estado de firmas, dashboard de bloqueos, reporting básico. *Límites: 1 centro, ≤250 prácticas/año, ≤500 alumnos, ≤500 empresas.*
- **Institution** — convenios marco, coverage por centro/programa/tipo, multi-coordinadora, roles y permisos, network activation, referral tracking, reporting avanzado. *≤5 centros, ≤1.000 prácticas, ≤3.000 alumnos/empresas.*
- **University Pro** — workflows avanzados, dashboards ejecutivos, reporting de empleabilidad, data exports, integración básica firma/documentos, customer success. *≤15 centros, ≤3.000 prácticas, ≤15.000 alumnos.*
- **Enterprise** — SSO, SIS/LMS/CRM/firma/documental, BI avanzado, auditoría, SLA, workflows configurables, rollout, CS dedicado. *Multi-campus, 8+ aplicativos coordinados.*

## Empresa — Internshiip for Employers
> Narrativa: **presencia institucional, relación continua y talento medible**. Nunca "publica gratis" ni "paga para promocionarte". Ver [[Posicionamiento y mensaje]].

| Plan | Anual | Pago mensual | Para quién |
|---|---|---|---|
| **Acceso operativo** | incluido por flujo | — | Empresas invitadas/colaboradoras de una institución |
| **Employer Presence** | 6.000 € | 600 € | Presencia institucional básica |
| **Employer Engagement** | 18.000 € | 1.800 € | Eventos, proyectos, retos, campañas |
| **Employer Network** | desde 60.000 € | custom | Gran empleador multi-sede/país |
| **Strategic Custom** | 60.000–150.000 € | custom | Campus talent como infraestructura |

## Fee por práctica activada (variable)
Existe pero **no es el titular público**. Permite facturar mensualmente por convenios firmados.
- **Evento facturable:** [[Entidad - SpecificAgreement|SpecificAgreement]] `fully_signed` y lista para inicio (=práctica activada).
- **Precio:** 39 € oficial · 29 € early adopter (12 meses) · 19 € ultra early (6 meses, primeros 3–5 logos).
- **Lenguaje de factura:** "Prácticas activadas — 18 × 39 €". Evitar "comisión", "success fee", "alumnos contratados".

## Early adopter / Founding Partner (año 1)
Descuento por confianza y co-creación, **no precio vitalicio**. Es la cara comercial del [[Founding Partner Program]].

| Plan | Oficial | Año 1 | Dto. |
|---|---|---|---|
| School | 13.000 € | **9.500 €** | −27% |
| Institution | 36.000 € | **24.000 €** | −33% |
| University Pro | 72.000 € | **48.000 €** | −33% |
| Employer Presence | 6.000 € | 3.600 € | −40% |
| Employer Engagement | 18.000 € | 12.000 € | −33% |

**Renovación:** el early adopter mantiene **20% sobre precio vigente** en la 1ª renovación si cumple feedback/adopción/referencia. No se congela el precio inicial.

## Fórmula de valor (conversación comercial)
`prácticas/año × horas administrativas/práctica × coste/hora = coste operativo manual`

| Ejemplo | Cálculo | Lectura |
|---|---|---|
| School | 250 × 4h × 25 € = **25.000 €/año** | Cuesta 13k. Recuperando la mitad del tiempo, se paga solo. |
| Institution | 1.000 × 4h × 25 € = **100.000 €/año** | Cuesta 36k. Captura una parte pequeña del coste que elimina. |
| University Pro | 3.000 × 4h × 25 € = **300.000 €/año** | Cuesta 72k. Upside en horas, coordinación, reporting, riesgo. |

## Evolución de precio a 3 años
Subida ligada a **valor probado**, nunca arbitraria.
- **Año 1 (validación):** precios base, early adopter 25–33%, fee 29–39 €.
- **Año 2 (producto probado):** +20–35% (School 16k / Institution 48k / Pro 90k / Enterprise desde 180k; Presence 9k; fee 49 €).
- **Año 3 (infra madura):** premium (School 20k / Institution 60k / Pro 110k / Enterprise desde 200k; fee 59–69 €).

## Público vs interno
- **Web pública:** orienta y cualifica, no es checkout. "Desde 1.083 €/mes (anual)" instituciones; "Employer Presence desde 500 €/mes". CTA: *Calcular ahorro operativo* / *Conocer Internshiip para empresas*. **No** mostrar "publica gratis", "success fee", "comisión" ni tabla de fee variable.
- **Interno:** matriz exacta para ventas/negociación. Suelos: School no bajar de 9.500 € salvo logo estratégico; Enterprise no vender sin discovery.

## Objeciones (resumen)
"Es caro" → compáralo con horas/errores/reporting manual, no con software · "Ya usamos firma/Excel" → la firma/Excel son piezas; faltan estado, responsable, bloqueo, trazabilidad, memoria · "La empresa no quiere pagar" → no paga para participar en el flujo; paga Presence/Engagement por relación · "¿Por qué mensual más caro?" → traslada riesgo y empeora caja. Detalle en [[Materiales de venta]].

Relacionado: [[Founding Partner Program]] · [[Modelo de monetización]] · [[Modelo RaaS]] · [[Métricas del caso de éxito]] · [[Roadmap 12 meses]]
